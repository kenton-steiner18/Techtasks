<!-- Getting Started -->
Events in the DOM
* Slide 1 (Syntax For Event Methods)
  * Introduce the comparison between the pure JavaScript and jQuery creating an event listener for "click".
    * document.getElementByclick("p").addEventListener("click", function, false); 
    * $("p").click(function() { // do something })
    * $("p").on("click", function() { // do something }); 

* Slide 2 (Common jQuery Event Methods)
  * create the event listener for "click" (example)
    * click() vs dblclick() 
  * create the event listener for "mouse" (example)
    * mouseenter() vs mouseleave() 
    * mousedown() vs mouseup()
    * hover()
  * create the event listener for "focus" (example)
    * focus() vs blur()

* Slide 3 (Event Propagation)
  * What is Event Propagation
  * preventDefault() method vs stopPropagation() method (example)

* Slide 4 (Event Delegation)
  * The behavior of Event Delegation (Syntax)
  * Why we need Event Delegation

* Slide 5 (Event Delegation cont.)
  * Delegated method
    * $("div").on("click", function(){...});
    * $(document).on("click", "div", function(){...});

* Slide 6 (Triggering an Event)
  * trigger() method vs triggerHandler() method 


