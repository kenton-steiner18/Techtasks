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
  * Insert Tree Picture
* Slide 3 (Tree Example cont.)
  * Insert the following code:
  * $(“div .university”); // => the span node under the div in class university
  * $(“.university”); // => A collection of all nodes in class university
  * $(“body h2”); // => ALL H2 nodes under BODY
  * $(“body > h2”); // => the H2 that is a direct child of BODY
  * $(“p.draft:nth-child(2)”); // => the IMG node which is the second child of the P tag in the class draft
  * $(“div h2,p”); // => Collection of the H2 node and the P node under the div
* Slide 4 (Tree Example Code rewritten)
  * $(“div”).find(“.university”);
  * $(“.university”); // This wouldn’t change because there is only one tag
  * $(“body”).find(“h2”); // Recall that this gets all children
  * $(“body”).children(“h2”); // This will get only DIRECT children
  * $(“p.draft”).nth-child(2);
  * $(“div”).find(“h2, p”);
* Slide 5 (jQuery selector methods)
  * .find()
  * .children()
  * .nth-child(n)
    * most pseudo-classes are also implemented as methods
  * jQuery methods or CSS selectors?
    * Used to be that jQuery methods were most optimal; however, more browsers implement document.querySelectorAll()
    * Results in a negligable performance upgrade
  * Method chaining can be more readable for long selectors
* Slide 6 (Walking the DOM)
  * .next([<selector>])
  * .prev([<selector>])
* Slide 7 (Traversing up the DOM)
  * .parent([<selector>])
  * .closest(<selector)
* Slide 8 (Tree example Picture again)
* Slide 9 (Tree Example - Walking/Traversing the DOM)
  * $(“img”).parent(); // => P node that is in the draft class
  * $(“img”).closest(“div”); // => DIV node that is in the warning class
  * $(“img”).prev(); // => A node that is the previous sibling of the IMG node
  * $(“div”).next().prev(); // => Same DIV node that we started with