## Quiz

*  Which of the following feature is not included in JQuery?  
	A. Modifying the DOM  
	B. Create Animation  
	C. Build Database  
	D. Support AJAX
*  Trace through the following HTML and JQuery code, what will the windown alert show?

``` 
<p id="test">This is some <b>bold</b> text in a paragraph.</p>

window.alert($("#test").html);
```

* 	Trace through the following HTML and JQuery code, what will be result of window alert when the user click `inner`? 

```
<p id="foo">outer</p>
<div>
	<p id= "foo">inner</p>
</div>

$("div").on("click","#foo",function(){
	var c = $(this).html() == "inner";
	alert("The result is " + c);
});
```  
