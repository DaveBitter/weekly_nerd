# To framework or not to framework?

This one of the discussions that I often see. I mostly work with React nowadays as my front-end framework. I'm a big fan of using React to create single page applications. But, I often find myself doing weird things to replicate functionality in HTML though.
```html
	<form method='POST' action='/upload'>
		<label>
			Full name *
			<input type='text' name='fullname' required='true' />
		</label>
		<label>
			Email address *
			<input type='email' name='email' required='true' />
		</label>
		<label>
			Date of birth *
			<input type='date' name='dateofbirth' required='true' />
		</label>
		<button type='submit' name='submit'>Send!</button>
	</form>
```
Forms are a perfect example of these things. Imagine a simple HTML form like the one above in a Node.js application. It will surprise you how many functionality this form has without Javascript not even taken CSS form validation in account. All I have to do is make a is handle the POST and I'm done. The a submit event is triggered by the submit button, the inputs will be validated and values will be passed along.

Imagine building this form in a framework like React. If I truly want this application to be single paged I will handle this form POST without actually posting.

Here is a list of functionalities to write to replace the HTML form functionality.

* `onChange` events for the inputs to save them in an object and re-render the input with that value. Each letter is an event that needs to be sent and added the value in the object. This will update the state which will the update the state which will then render the input with the new value
* Check to see if all required inputs are filled in
* Write form validation for each type of input

That's a lot of Javascript. If my Javascript breaks one of the most basic functionalities of a website breaks. Is this the right way to build my application then?

Yes, yes it is. I know that this sounds stupid. If this works this way then why not ditch it and revert back to the good old POST form. If this is all the functionality then I should just `preventDefault()` the submit of the form and to a client-side POST to the server. No, if I am going to use React for a form I'm going to enhance the functionality. Something like showing users that somebody else is also updating the values in that form. I can even add simultaneously form editing with other users.

In my opinion this is what we should use frameworks for. To build functionality that isn't otherwise achieved in an evenly simple manner. We've got these cool frameworks which we mostly then use to reinvent the wheel. *Let's supercharge that wheel with the tools that are available today*! Sure use the most basic and simplest form of providing you're functionality, but don't be afraid to make new functionality.
