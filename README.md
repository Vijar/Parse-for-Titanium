Parse-for-Titanium
==================

Use the Parse Javascript SDK with Titanium Studio.

Versions
-------------------------

Parse Javascript SDK 1.1.4

Titanium Studio 2.1

Installation
-------------------------

1. Copy the included parse-x.x.x.js file into the "Resources" folder in Titanium

2. Copy the following line to the top of "app.js" in your project "Resources" folder

	<pre>Ti.include("parse-1.1.4.js");</pre>

3. Just use parse like you would normally using the [Parse Javascript SDK Guide]()

	i.e. add this to your code to test if its working

	<pre>
	Parse.initialize(applicationId, javaScriptKey);

	var TestObject = Parse.Object.extend("TestObject");
	var testObject = new TestObject();
	testObject.save({foo: "bar"}, {
	  success: function(object) {
	    alert("yay! it worked");
	  }
	});
	</pre>