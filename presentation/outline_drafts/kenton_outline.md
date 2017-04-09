<!-- AJAX -->
*Slide 1 (What is AJAX?)
  *AJAX: Asynchronous JavaScript and XML
  * Use of XmlHttpRequest objects to interact with web server dynamically via Javascript
  * Faster data exchange method with server
  * Single line of Code
* Slide 2 (jQuery AJAX Implementation)
  * 2 Methods
    * .ajax() method
    * Convenience functions: 
      *.get()
      *.post()
* Slide 3 (The Heart of It All)
  * .ajax() method
    * Takes a parameter of a configuration object
    * Allows for many more configuration options
      * Options include: url, data, type, dataType, done, fail, always
* Slide 4 (.ajax() example) 
  * $.ajax({
      url: "post.php", //URL for the request message 
      data: {id: 100}, //Data to be sent in request
      type: "GET",//Whether this is a POST or GET request 
      dataType: "json",//Type of data expected to be returned
    })
    //Code to run if request succeeds
    .done(function(json) {
      // callback function
    })
* Slide 5 (For your Convenience)
  * .get() 
    * $.get(URL,callback);
    * sends HTTP GET request to server
  * .post()
    * $.post(URL,data,callback);
    * requests data from server using HTTP POST request
* Slide 6 (Get and Post examples)
  * $.get("all_this_data.html", function(data,status){ //Callback function definition })
  * $.post("all_this_data.html", { name: "Fred" greeting: "Hello World!" },
  function(data,status){ //Callback function definition })
* Slide 7 (Pick Your Poison)
  * How to determine what method to use? 
    * Convenience Functions: 
      * Sending simple requests
      * Default settings are OK
    * .ajax()
      * Perform error handling
      * Single point of Control
      * Extensive configuration of requests
