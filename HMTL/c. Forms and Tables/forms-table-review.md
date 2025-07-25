### HTML Tables and Forms Review
## HTML Form Elements and Attributes

- `form` element: used to create an HTML form for user input.
- `action` attribute: used to specify the URL where the form data should be sent.
- `method` attribute: used to specify the HTTP method to use when sending the form data. The most common methods are `GET` and `POST`.

Example Code
```html
<form method="value-goes-here" action="url-goes-here">
  <!-- inputs go inside here -->
</form>
```

- `input` element: used to create an input field for user input.
- `type` attribute: used to specify the type of input field. Ex. `text`, `email`, `number`, `radio`, `checkbox`, etc.
- `placeholder` attribute: used to show a hint to the user to show them what to enter in the input field.
- `value` attribute: used to specify the value of the input. If the input has a button type, the value attribute can be used to set the `button` text.
- `name` attribute: used to assign a name to an input field, which serves as the key when form data is submitted. For radio buttons, giving them the same `name` groups them together, so only one option in the group can be selected at a time.
- `size` attribute: used to define the number of characters that should be visible as the user types into the input.
- `min` attribute: can be used with input types such as `number` to specify the minimum value allowed in the input field.
- `max` attribute: can be used with input types such as `number` to specify the maximum value allowed in the input field.
- `minlength` attribute: used to specify the minimum number of characters required in an input field.
- `maxlength` attribute: used to specify the maximum number of characters allowed in an input field.
- `required` attribute: used to specify that an input field must be filled out before submitting the form.
- `disabled` attribute: used to specify that an input field should be disabled.
- `readonly` attribute: used to specify that an input field is read-only.

Example Code
```html
<!-- Text input -->
<input 
  type="text"
  id="name"
  name="name"
  placeholder="e.g. Quincy Larson" 
  size="20"
  minlength="5"
  maxlength="30"
  required
/>

<!-- Number input -->
<input 
  type="number"
  id="quantity"
  name="quantity"
  min="2"
  max="10"
  disabled
/>

<!-- Button -->
<input type="button" value="Show Alert" />
```

- `label` element: used to create a label for an input field.
- `for` attribute: used to specify which input field the label is for.
- `Implicit form association`: inputs can be associated with labels by wrapping the input field inside the label element.

Example Code
```html
<form action="">
  <label>
    Full Name:
    <input type="text" />
  </label>
</form>
```

- `Explicit form association`: inputs can be associated with labels by using the for attribute on the label element.

Example Code
```html
<form action="">
  <label for="email">Email Address: </label>
  <input type="email" id="email" />
</form>
```

- `button` element: used to create a clickable button. A button can also have a `type` attribute, which is used to control the behavior of the button when it is activated. Ex. `submit`, `reset`, `button`.

Example Code
```html
<button type="button">Show Form</button>
<button type="submit">Submit Form</button>
<button type="reset">Reset Form</button>
```

- `fieldset` element: used to group related inputs together.
- `legend` element: used to add a caption to describe the group of inputs.
Example Code
```html
<!-- Radio group -->
<fieldset>
  <legend>Was this your first time at our hotel?</legend>

  <label for="yes-option">Yes</label>
  <input id="yes-option" type="radio" name="hotel-stay" value="yes" />

  <label for="no-option">No</label>
  <input id="no-option" type="radio" name="hotel-stay" value="no" />
</fieldset>

<!-- Checkbox group -->
<fieldset>
  <legend>
    Why did you choose to stay at our hotel? (Check all that apply)
  </legend>

  <label for="location">Location</label>
  <input type="checkbox" id="location" name="location" value="location" />

  <label for="price">Price</label>
  <input type="checkbox" id="price" name="price" value="price" />
</fieldset>
```

- `Focused state`: this is the state of an input field when it is selected by the user.

### Working with HTML Table Elements and Attributes

- **Table element**: used to create an HTML table.
- **Table Head (`thead`) element**: used to group the header content in an HTML table.
- **Table Row (`tr`) element**: used to create a row in an HTML table.
- **Table Header (`th`) element**: used to create a header cell in an HTML table.
- **Table body (`tbody`) element**: used to group the body content in an HTML table.
- **Table Data Cell (`td`) element**: used to create a data cell in an HTML table.
- **Table Foot (`tfoot`) element**: used to group the footer content in an HTML table.
- **`caption` element**: used to add a title of an HTML table.
- **`colspan` attribute**: used to specify the number of columns a table cell should span.

Example Code
```html
<table>
  <caption>Exam Grades</caption>

  <thead>
    <tr>
      <th>Last Name</th>
      <th>First Name</th>
      <th>Grade</th>
    </tr>
  </thead>

  <tbody>
    <tr>
      <td>Davis</td>
      <td>Alex</td>
      <td>54</td>
    </tr>

    <tr>
      <td>Doe</td>
      <td>Samantha</td>
      <td>92</td>
    </tr>

    <tr>
      <td>Rodriguez</td>
      <td>Marcus</td>
      <td>88</td>
    </tr>
  </tbody>

  <tfoot>
    <tr>
      <td colspan="2">Average Grade</td>
      <td>78</td>
    </tr>
  </tfoot>
</table>
```

### Working with HTML Tools
- **HTML validator**: a tool that checks the syntax of HTML code to ensure it is valid.
- **DOM inspector**: a tool that allows you to inspect and modify the HTML structure of a web page.
- **Devtools**: a set of web developer tools built directly into the browser that helps you debug, profile, and analyze web pages.