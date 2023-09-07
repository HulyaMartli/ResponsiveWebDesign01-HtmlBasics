# HTML5

* Only use one h1 element per page.
* All img elements should have an alt attribute. The alt attribute's text is used for screen readers to improve accessibility and is displayed if the image fails to load.
* The figure element represents self-contained content and will allow you to associate an image with a caption. A figure caption (figcaption) element is used to add a caption to describe the image contained within the figure element. 
* The \<em> HTML element marks text that has stress emphasis.
* The strong element is used to indicate that some text is of strong importance or urgent.

## Forms

* In order for a form's data to be accessed by the location specified in the action attribute, you must give the text field a name attribute and assign it a value to represent the data being submitted

* To prevent a user from submitting your form when required information is missing, you need to add the required attribute to an input element.

* The default behavior of clicking a form button without any attributes submits the form to the location specified in the form's action attribute. However, relying on default behavior may cause confusion. Add the type attribute with the value submit to the button to make it clear that it is a submit button.

* You can use radio buttons for questions where you want only one answer out of multiple options.

* label elements are used to help associate the text for an input element with the input element itself (especially for assistive technologies like screen readers). For example, <label><input type="radio"> cat</label> makes it so clicking the word cat also selects the corresponding radio button.

* The id attribute is used to identify specific HTML elements. Each id attribute's value **must be unique** from **all other id values** ***for the entire page***.

* To make it so selecting one radio button automatically deselects the other, both buttons must have a name attribute with the same value.

* When radio buttons do not have a value attribute, the form data will include nameGiven=on (e.g. indoor-outdoor=on), which is not useful when you have multiple buttons. So we should add a value attribute (e.g. value="indoor")

* The **fieldset element** is used to group related inputs and labels together in a web form. fieldset elements are block-level elements, meaning that they appear on a new line.

* The **legend element** acts as a caption for the content in the fieldset element. It gives users context about what they should enter into that part of the form.

* There's another way to associate an input element's text with the element itself. You can nest the text within a **label element** and add a **for attribute** with the **same value as the input element's id attribute**.    

  ~~~~
  <input id="loving" type="checkbox"> <label for="loving"> Loving </label>
  ~~~~

  (There should be a space between input and label elements)

* While you won't notice this in the browser, **adding name attribute** makes it easier for a server to process your web form, especially when there are multiple checkboxes.

* Like radio buttons, **form data for selected checkboxes are name / value attribute pairs**. While the value attribute is optional, ***it's best practice to include it with any checkboxes or radio buttons on the page***.

* In order to make a checkbox checked or radio button selected by default, you need to add the **checked attribute** to it.

* You can **set browser behavior** by adding self-closing ***meta elements*** in the head (e.g. Tell the browser to parse the markup into multiple languages by creating a meta element as a child of the head element. Set its charset attribute to UTF-8.)