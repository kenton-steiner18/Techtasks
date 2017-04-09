<!-- Getting Started -->

* Slide 1 (Getting Started)
  * Two ways to add jQuery to your projects:
    * download from jQuery.com/download
    * CDN (Content Delivery Network) [Preferred]
* Slide 2
  * Where to include script tag?
    * <body>
      * end of <body>
    *<head>
      * Wrap in document.ready
    * Both work! 

<!-- If you do neither, event handlers won't work because the tags they are assigned to won't have been created in the DOM -->

<!-- Maneuvering the DOM -->

* Slide 1 (Maneuvering the DOM)
  * $(<selector>)
    * CSS selector: .class, #id, :pseudo-classes, and <html> tag (not ::pseudo-elements)
  * Pure JS code:
    * document.getElementsBy(“ul”);
	* document.getElementsByClassName(“highlight”);
	* document.getElementById(“footer”);
  * jQuery code:
    * $(“ul”);
	* $(“.highlight”);
	* $(“#footer”);
  * "" vs ''?
    * jQuery Core Style Guide
* Slide 2 (Tree Example)
  * (Insert tree into jsFiddle and run examples)

<!-- Create HTML code for tree example as well so we can play with jsFiddle -->

* Slide 3 (Tree Example cont.)
  * .find()
  * .children()
  * .nth-child(n)
    * most pseudo-classes are also implemented as methods
  * jQuery methods or CSS selectors?
    * Used to be that jQuery methods were most optimal; however, more browsers implement document.querySelectorAll()
    * Results in a negligable performance upgrade
  * Method chaining can be more readable for long selectors
* Slide 4 (Walking the DOM)
  * .next([<selector>])
  * .prev([<selector>])
* Slide 5 (Traversing up the DOM)
  * .parent([<selector>])
  * .closest(<selector)
  * (Create another jsFiddle with the tree example)
* Slide 6 (Tree example Picture again)