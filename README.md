# Day-10-Class-work
In this Project we have a Circle and inside the circle we have two shape first one is trangle and reactangle and we can change the background of the circle and also change the shape.
In is Project we using DOM manipulation and Event Listener.
First of all we take a div (container) after that and inside the container div we take three div -: (circlr , change-color , and change-shape) after  that we apply flex box property in css part and add sub basic css .
In the JS part first of all we take a sum color for the circlr and after that we get the element in JS using :-
                  var cShape = document.getElementById("change-shape");
                  var cColor = document.getElementById("change-color");
                  
And Apply EventListener function :-
                 cShape.addEventListener("click", changeShape);
                 cColor.addEventListener("click", changeColor);
                 
and write the function color change and apply If else condition in the if part 
(index === color.length)
 document.getElementById("circle").style.backgroundColor = color[index];
    index++;
And write anoter function changeShape :-
 if (!isTriangle) {
      var i = document.getElementsByClassName("inner")[0];
      i.className = "triangle-bottom-left";
      isTriangle = true;
    }else{
      var i = document.getElementsByClassName("triangle-bottom-left")[0];
      i.className = "inner";
      isTriangle = false;
    }
