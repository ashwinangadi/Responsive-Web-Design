# Learn HTML by Building a cat Photo App
### Steps that are included to build a cat photo app, we learn all basics of HTML by completing this assignment.

## **Step 1**
HTML elements have opening tags like `<h1>` and closing tags like `</h1>`.<br>

The text for an element goes between its opening and closing tags.<br>

Find the `h1` element and change its text to:<br>

`CatPhotoApp`

```html
<h1>CatPhotoApp</h1> 
```


## **Step 2**
The `h1` through `h6` heading elements are used to signify the importance of content below them.<br>
The lower the number, the higherthe importance, so `h2` elements have less importance than `h1` elements.<br>
Only use one `h1` element per page and place lower importance headings below higher importance headings.<br>

Below the `h1` element, add an `h2` element with this text:<br>

`Cat Photos`

```html
<h1>CatPhotoApp</h1>
<h2>Cat Photos</h2>
```


## **Step 3**
The `p` element is used to create a paragraph of text on websites.<br>
Create a `p` element below your `h2` element and give it the following text:<br>

`Click here to view more cat photos.`

```html
<h2>Cat Photos</h2>
<p>Click here to view more cat photos</p>
```
## **Step 4**
Commenting allows you to leave messages without affecting the browser display.<br>
It also allows you to make code inactive. A comment in HTML starts with `<!--`, contains any number of lines of text, and ends with `-->`.<br> 
For example, the comment `<!-- TODO: Remove h1 -->` contains the text TODO: Remove h1.<br>

Add a comment above the p element with this text:<br>

`TODO: Add link to cat photos`

```html
<!-- TODO: Add link to cat photos -->
<p>Click here to view more cat photos.</p>
```
## **Step 5**
HTML5 has some elements that identify different content areas. <br>
These elements make your HTML easier to read and help with Search Engine Optimization (SEO) and accessibility.<br>

Identify the main section of this page by adding a `<main>` opening tag before the `h1` element, and a `</main>` closing tag after the `p` element.<br>

```html
<main>
      <h1>CatPhotoApp</h1>
      <h2>Cat Photos</h2>
      <!-- TODO: Add link to cat photos -->
    <p>Click here to view more cat photos.</p>
</main>
```
## **Step 6**
In the previous step, you put the `h1`, `h2`, comment, and `p` elements inside the `main` element.<br>
This is called nesting. Nested elements should be placed two spaces further to the right of the element they are nested in.<br>
This spacing is called indentation and it is used to make HTML easier to read.<br>

The `h1` element, `h2` element and the comment are indented two spaces more than the `main` element in the code below.<br>
Use the space bar on your keyboard to add two more spaces in front of the `p` element so that it is indented properly as well.<br>

```html
<main>
      <h1>CatPhotoApp</h1>
      <h2>Cat Photos</h2>
      <!-- TODO: Add link to cat photos -->
      <p>Click here to view more cat photos.</p>
</main>
```
## **Step 7**
You can add images to your website by using the `img` element.<br>
`img` elements have an opening tag without a closing tag.<br>
A tag for an element without a closing tag is known as a self-closing tag.<br>

Add an `img` element below the `p` element. At this point, no image will show up in the browser.<br>

```html
<p>Click here to view more cat photos.</p>
<img />
```
## **Step 8**
HTML attributes are special words used inside the opening tag of an element to control the element's behavior.<br>
The `src` attribute in an `img` element specifies the image's URL (where the image is located).<br>
An example of an `img` element using an `src` attribute: `<img src="https://www.example.com/the-image.jpg">.`<br>

Inside the existing `img` element, add an `src` attribute with this URL:<br>

`https://cdn.freecodecamp.org/curriculum/cat-photo-app/relaxing-cat.jpg`<br>

```html
<img src="https://cdn.freecodecamp.org/curriculum/cat-photo-app/relaxing-cat.jpg" />
```
## **Step 9**
All `img` elements should have an `alt` attribute. <br>
The `alt` attribute's text is used for screen readers to improve accessibility and is displayed if the image fails to load. <br>
For example, `<img src="cat.jpg" alt="A cat">` has an `alt` attribute with the text `A cat`.<br>

Inside the `img` element, add an `alt` attribute with this text:<br>

`A cute orange cat lying on its back`<br>

```html
<img src="https://cdn.freecodecamp.org/curriculum/cat-photo-app/relaxing-cat.jpg"
  alt="A cute orange cat lying on its back" />

```
## **Step 10**
You can link to another page with the anchor `(a)` element.<br> 
For example, `<a href='https://freecodecamp.org'></a>` would link to freecodecamp.org.<br>

Add an anchor element after the paragraph that links to `https://freecatphotoapp.com`. <br>
At this point, the link won’t show up in the preview.<br>

```html
<p>Click here to view more cat photos.</p>
<a href="https://freecatphotoapp.com"></a>
```
## **Step 11**
A link's text must be placed between the opening and closing tags of an anchor `(a)` element. <br>
For example, `<a href="https://www.freecodecamp.org">click here to go to freeCodeCamp.org</a>` is a link with the text `click here to go to freeCodeCamp.org`.<br>

Add the anchor text `link to cat pictures` to the anchor element. <br>
This will become the link's text.<br>

```html
<a href="https://freecatphotoapp.com">link to cat pictures</a>
```
## **Step 12**
In the previous step you turned the words `link to cat pictures` into a link by placing them between opening and closing anchor `(a)` tags.<br> 
You can do the same to words inside of an element, such as a `p` element.<br>

In the text of your p element, turn the words `cat photos` into a link to `https://freecatphotoapp.com`<br>
by adding opening and closing anchor `(a)` tags around these words.<br>

```html
<p>Click here to view more <a href="https://freecatphotoapp.com">cat photos</a></p>
```
## **Step 13**
Now that you turned the text `cat photos` inside the `p` element into a link, you don't need the second link below the `p` element. <br>
Delete the entire anchor element below the `p` element.<br>

```html
<p>
  Click here to view more
  <a href="https://freecatphotoapp.com" target="_blank">cat photos</a>.
</p>
```
## **Step 14**
Add a `target` attribute with the value `_blank` to the anchor `(a)` element's opening tag, <br>
so that the link opens in a new tab.<br>

```html
<p>Click here to view more <a href="https://freecatphotoapp.com" target="_blank">cat photos</a>.</p>
```
## **Step 15**
Turn the image into a link by surrounding it with necessary element tags.<br> 
Use `https://freecatphotoapp.com` as the anchor's `href` attribute value.<br>

```html
<a href="https://freecatphotoapp.com"><img src="https://cdn.freecodecamp.org/curriculum/cat-photo-app/relaxing-cat.jpg" alt="A cute orange cat lying on its back."></a>

```
## **Step 16**
Before adding any new content, you should make use of a `section` element to separate the cat photos content from the future content.<br>

Take your `h2`, comment, `p`, and anchor `(a)` elements and nest them in a `section` element.<br>

```html
      <section>
        <h2>Cat Photos</h2>
        <!-- TODO: Add link to cat photos -->
        <p>Click here to view more <a target="_blank" href="https://freecatphotoapp.com">cat photos</a>.</p>
        <a href="https://freecatphotoapp.com"><img src="https://cdn.freecodecamp.org/curriculum/cat-photo-app/relaxing-cat.jpg" alt="A cute orange cat lying on its back."></a>
     </section>
```
## **Step 17**
It is time to add a new section. Add a second `section` element below the existing `section` element.<br>

```html
</section>
  <section>
        
  </section>
```
## **Step 18**
Within the second `section` element, add a new `h2` element with the text `Cat Lists`.<br>

```html
<section>
  <h2>Cat Lists</h2>
</section>
```
## **Step 19**
When you add a lower rank heading element to the page, it's implied that you're starting a new subsection.<br>

After the last `h2` element of the second `section` element, add an `h3` element with this text:<br>

`Things cats love:`<br>

```html
<section>
 <h2>Cat Lists</h2>
 <h3>Things cats love:</h3>
</section>
```
## **Step 20**
After the `h3` element with the `Things cats love:` text, add an unordered list `(ul)` element.<br> 
Note that nothing will be displayed at this point.<br>

```html
<h3>Things cats love:</h3>
<ul>
          
</ul>
```
## **Step 21**
Use list item `(li)` elements to create items in a list. Here is an example of list items in an unordered list:<br>
```html
<ul>
  <li>milk</li>
  <li>cheese</li>
</ul>
```
Within the `ul` element nest three list items to display three things cats love:<br>

`cat nip`, `laser pointers`, `lasagna`<br>

```html
<ul>
  <li>cat nip</li>
  <li>laser pointers</li>
  <li>lasagna</li>
</ul>
```
## **Step 22**
After the unordered list, add a new image with an `src` attribute value set to:<br>

`https://cdn.freecodecamp.org/curriculum/cat-photo-app/lasagna.jpg`<br>

And its `alt` attribute value to:<br>

`A slice of lasagna on a plate.`<br>

```html
<ul>
  <li>cat nip</li>
  <li>laser pointers</li>
  <li>lasagna</li>
</ul>
<img src="https://cdn.freecodecamp.org/curriculum/cat-photo-app/lasagna.jpg" alt="A slice of lasagna on a plate.">
```
## **Step 23**
The `figure` element represents self-contained content and will allow you to associate an image with a caption.<br>

Nest the image you just added within a `figure` element.<br>

```html
<figure>
  <img src="https://cdn.freecodecamp.org/curriculum/cat-photo-app/lasagna.jpg" alt="A slice of lasagna on a plate.">
</figure>
```
## **Step 24**
A figure caption (`figcaption`) element is used to add a caption to describe the image contained within the `figure` element.<br> 
For example, `<figcaption>A cute cat</figcaption>` adds the caption `A cute cat`.<br>

After the image nested in the `figure` element, add a `figcaption` element with text set to:<br>

`Cats love lasagna.`<br>

```html
<figure>
  <img src="https://cdn.freecodecamp.org/curriculum/cat-photo-app/lasagna.jpg" alt="A slice of lasagna on a plate.">
  <figcaption>Cats love lasagna</figcaption>
</figure>
```
## **Step 25**
Emphasize the word `love` in the `figcaption` element by wrapping it in an emphasis `em` element.<br>

```html
<figcaption>Cats <em>love</em> lasagna.</figcaption>
```
## **Step 26**
After the `figure` element, add another `h3` element with the text:<br>

`Top 3 things cats hate:`<br>

```html
  </figure>
  <h3>Top 3 things cats hate:</h3>
</section>
```
## **Step 27**
The code for an ordered list (`ol`) is similar to an unordered list, but list items in an ordered list are numbered when displayed.<br>

After the second `section` element's last `h3` element, add an ordered list with these three list items:<br>

`flea treatment`, `thunder`, `other cats`

```html
<h3>Top 3 things cats hate:</h3>
  <ol>
      <li>flea treatment</li>
      <li>thunder</li>
      <li>other cats</li>
    </ol>
```
## **Step 28**
After the ordered list, add another `figure` element.<br>

```html
</ol>
<figure>
  
</figure>
```
## **Step 29**
Inside the `figure` element you just added, nest an `img` element with a `src` attribute set to<br> 
`https://cdn.freecodecamp.org/curriculum/cat-photo-app/cats.jpg.`<br>

```html
<figure>
  <img src="https://cdn.freecodecamp.org/curriculum/cat-photo-app/cats.jpg">
</figure>
```
## **Step 30**
To improve accessibility of the image you just added, add an `alt` attribute with the text:<br>

`Five cats looking around a field.`

```html
<figure>
  <img src="https://cdn.freecodecamp.org/curriculum/cat-photo-app/cats.jpg" alt="Five cats looking around a field.">
</figure>
```
## **Step 31**
After the last `img` element, add a `figcaption` element with the text `Cats hate other cats.`<br>

```html
<figure>
  <img src="https://cdn.freecodecamp.org/curriculum/cat-photo-app/cats.jpg" alt="Five cats looking around a field.">
  <figcaption>Cats hate other cats.</figcaption>
</figure>
```
## **Step 32**
The `strong` element is used to indicate that some text is of strong importance or urgent.<br>

In the `figcaption` you just added, indicate that `hate` is of strong importance by wrapping it in a `strong` element.

```html
<figcaption>Cats <strong>hate</strong> other cats.</figcaption>  
```
## **Step 33**
It is time to add a new section. Add a third `section` element below the second `section` element.<br>

```html
</section> //second section
  <section>

  </section>
```
## **Step 34**
Inside the third `section` element, add an `h2` element with the text:<br>

`Cat Form`

```html
<section>
  <h2>Cat Form</h2>
</section>
```
## **Step 35**
Now you will add a web form to collect information from users.<br>

After the `Cat Form` heading, add a `form` element.

```html
<h2>Cat Form</h2>
<form>
          
</form>
```
## **Step 36**
The `action` attribute indicates where form data should be sent. <br>
For example, `<form action="/submit-url"></form>` tells the browser that the form data should be sent to the path `/submit-url.`<br>

Add an `action` attribute with the value `https://freecatphotoapp.com/submit-cat-photo` to the `form` element.

```html
<form action="https://freecatphotoapp.com/submit-cat-photo">
</form>
```
## **Step 37**
The `input` element allows you several ways to collect data from a web form. <br>
Like `img` elements, `input` elements are self-closing and do not need closing tags.<br>

Nest an `input` element in the `form` element.

```html
<form action="https://freecatphotoapp.com/submit-cat-photo">
<input>
</form>
```
## **Step 38**
There are many kinds of inputs you can create using the `type` attribute. <br>
You can easily create a password field, reset button, or a control to let users select a file from their computer.<br>

Create a text field to get text input from a user by adding the `type` attribute with the value `text` to the `input` element.

```html
<form action="https://freecatphotoapp.com/submit-cat-photo">
<input type="text">
</form>
```
## **Step 39**
In order for a form's data to be accessed by the location specified in the `action` attribute, <br>
you must give the text field a `name` attribute and assign it a value to represent the data being submitted.<br> 
For example, you could use the following syntax for an email address text field: `<input type="text" name="email">`.<br>

Add the `name` attribute with the value `catphotourl` to your text field.

```html
<input type="text" name="catphotourl">
```
## **Step 40**
Placeholder text is used to give people a hint about what kind of information to enter into an input. <br>
For example, `<input type="text" placeholder="Email address">`.<br>

Add the placeholder text `cat photo URL` to your `input` element.

```html
<input type="text" name="catphotourl" placeholder="cat photo URL">
```
## **Step 41**
To prevent a user from submitting your form when required information is missing, you need <br>
to add the `required` attribute to an `input` element. There's no need to set a value to the `required` attribute. <br>
Instead, just add the word `required` to the `input` element, making sure there is space between it and other attributes.

```html
<input type="text" name="catphotourl" placeholder="cat photo URL" required>
```
## **Step 42**
Use the `button` element to create a clickable button. For example, `<button>Click Here</button>` creates a button with the text `Click Here.`<br>

Add a `button` element with the text `Submit` below the `input` element. The default behavior of clicking a form button <br>
without any attributes submits the form to the location specified in the form's `action` attribute.

```html
<input type="text" name="catphotourl" placeholder="cat photo URL" required>
<button>Submit</button>
```
## **Step 43**
Even though you added your button below the text input, they appear next to each other on the page. <br>
That's because both `input` and `button` elements are inline elements, which don't appear on new lines.<br>

The button you added will submit the form by default. However, relying on default behavior may cause confusion. <br>
Add the `type` attribute with the value `submit` to the `button` to make it clear that it is a submit button.

```html
<button type="submit">Submit</button>
```
## **Step 44**
You can use radio buttons for questions where you want only one answer out of multiple options.<br>

Here is an example of a radio button with the option of `cat`: `<input type="radio"> cat`. Remember that `input` elements are self-closing.<br>

Before the text input, add a radio button with the option set as:<br>

`Indoor`

```html
<form action="https://freecatphotoapp.com/submit-cat-photo">
  <input type="radio"> Indoor
  <input type="text" name="catphotourl" placeholder="cat photo URL" required>
  <button type="submit">Submit</button>
</form>
```
## **Step 45**
`label` elements are used to help associate the text for an `input` element with the `input` element itself <br>
(especially for assistive technologies like screen readers). <br>
For example, `<label><input type="radio"> cat</label>` makes it so clicking the word `cat` also selects the corresponding radio button.<br>

Nest your `radio` button inside a `label` element.

```html
<label> <input type="radio"> Indoor </label>
```
## **Step 46**
The `id` attribute is used to identify specific HTML elements. Each `id` attribute's value must be unique from all other `id` values for the entire page.<br>

Add an `id` attribute with the value `indoor` to the radio button. When elements have multiple attributes, the order of the attributes doesn't matter.

```html
<label><input type="radio" id="indoor"> Indoor</label>
```
## **Step 47**
Create another radio button below the first one. Nest it inside a `label` element with `Outdoor` as the `label` text. <br>
Give the radio button an `id` attribute with `outdoor` as the value.

```html
<label><input id="indoor" type="radio"> Indoor</label>
<label><input id="outdoor" type="radio"> Outdoor</label>
```
## **Step 48**
Notice that both radio buttons can be selected at the same time. <br>
To make it so selecting one radio button automatically deselects the other, both buttons must have a `name` attribute with the same value.<br>

Add the `name` attribute with the value `indoor-outdoor` to both radio buttons.

```html
<label><input id="indoor" name="indoor-outdoor" type="radio"> Indoor</label>
<label><input id="outdoor" name="indoor-outdoor" type="radio"> Outdoor</label>
```
## **Step 49**
If you select the `Indoor` radio button and submit the form, the form data for the button is based on its `name` and `value` attributes. <br>
Since your radio buttons do not have a `value` attribute, the form data will include `indoor-outdoor=on`, which is not useful when you have multiple buttons.<br>

Add a `value` attribute to both radio buttons. For convenience, set the button's `value` attribute to the same value as its `id` attribute.

```html
<label><input id="indoor" value="indoor" type="radio" name="indoor-outdoor"> Indoor</label>
<label><input id="outdoor" value="outdoor" type="radio" name="indoor-outdoor"> Outdoor</label>
```
## **Step 50**
The `fieldset` element is used to group related inputs and labels together in a web form. <br>
`fieldset` elements are block-level elements, meaning that they appear on a new line.<br>

Nest the `Indoor` and `Outdoor` radio buttons within a `fieldset` element, and don't forget to indent the radio buttons.

```html
<fieldset>
  <label><input id="indoor" type="radio" name="indoor-outdoor" value="indoor"> Indoor</label>
  <label><input id="outdoor" type="radio" name="indoor-outdoor" value="outdoor"> Outdoor</label>
</fieldset>
```
## **Step 51**
The `legend` element acts as a caption for the content in the `fieldset` element. <br>
It gives users context about what they should enter into that part of the form.<br>

Add a `legend` element with the text `Is your cat an indoor or outdoor cat?` above both of the radio buttons.

```html
<fieldset>
  <legend>Is your cat an indoor or outdoor cat?</legend>
  <label><input id="indoor" type="radio" name="indoor-outdoor" value="indoor"> Indoor</label>
  <label><input id="outdoor" type="radio" name="indoor-outdoor" value="outdoor"> Outdoor</label>
</fieldset>
```
## **Step 52**
Next, you are going to add some new form `input` elements, so add another `fieldset` element directly below the current `fieldset` element.<br>

```html
</fieldset>// first element
  <fieldset>
            
  </fieldset>
```
## **Step 53**
Add a `legend` element with the text `What's your cat's personality?` inside the second `fieldset` element.

```html
<fieldset>
  <legend>What's your cat's personality?</legend>
</fieldset>
```
## **Step 54**
Forms commonly use checkboxes for questions that may have more than one answer. <br>
For example, here's a checkbox with the option of `tacos`: `<input type="checkbox"> tacos`.<br>

Under the `legend` element you just added, add an `input` with its `type `attribute set to `checkbox` and give it the option of:<br>

`Loving`

```html
<fieldset>
  <legend>What's your cat's personality?</legend>
  <input type="checkbox"> Loving
</fieldset>
```
## **Step 55**
Add an `id` attribute with the value `loving` to the checkbox input.

```html
<input type="checkbox" id="loving"> Loving
```
## **Step 56**
There's another way to associate an `input` element's text with the element itself.<br> 
You can nest the text within a `label` element and add a `for` attribute with the same value as the `input` element's `id` attribute.<br>

Associate the text `Loving` with the checkbox by only nesting the text `Loving` in a `label` element and place it to the right side of the checkbox `input` element.

```html
<input id="loving" type="checkbox"> <label for="loving">Loving</label>
```
## **Step 57**
Add the `name` attribute with the value `personality` to the checkbox `input` element.<br>

While you won't notice this in the browser, doing this makes it easier for a server to process your web form, especially when there are multiple checkboxes.

```html
<input id="loving" type="checkbox" name="personality"> <label for="loving">Loving</label>
```
## **Step 58**
Add another checkbox after the one you just added. <br>
The `id` attribute value should be `lazy` and the `name` attribute value should be the same as the last checkbox.<br>

Also add a `label` element to the right of the new checkbox with the text `Lazy`.<br> 
Make sure to associate the `label` element with the new checkbox using the `for` attribute.

```html
<input id="loving" type="checkbox" name="personality"> <label for="loving">Loving</label>
<input id="lazy" type="checkbox" name="personality"> <label for="lazy">Lazy</label>
```
## **Step 59**
Add a final checkbox after the previous one with an `id` attribute value of `energetic`. The `name` attribute should be the same as the previous checkbox.<br>

Also add a `label` element to the right of the new checkbox with text `Energetic`. Make sure to associate the `label` element with the new checkbox.

```html
<fieldset>
  <legend>What's your cat's personality?</legend>
  <input id="loving" type="checkbox" name="personality"> <label for="loving">Loving</label>
  <input id="lazy" type="checkbox" name="personality"> <label for="lazy">Lazy</label>
  <input id="energetic" type="checkbox" name="personality"> <label for="energetic">Energetic</label>
</fieldset>
```
## **Step 60**
Like radio buttons, form data for selected checkboxes are `name` / `value` attribute pairs. <br>
While the `value` attribute is optional, it's best practice to include it with any checkboxes or radio buttons on the page.<br>

Add a `value` attribute to each checkbox. For convenience, set each checkbox's `value` attribute to the same value as its `id` attribute.

```html
<input id="loving" type="checkbox" name="personality" value="loving"> <label for="loving">Loving</label>
<input id="lazy" type="checkbox" name="personality" value="lazy"> <label for="lazy">Lazy</label>
<input id="energetic" type="checkbox" name="personality" value="energetic"> <label for="energetic"> Energetic</label>
```
## **Step 61**
In order to make a checkbox checked or radio button selected by default, you need to add the `checked` attribute to it. <br>
There's no need to set a value to the `checked` attribute. Instead, just add the word `checked` to the `input` element, making sure there is space between it and other attributes.<br>

Make the first radio button and the first checkbox selected by default.

```html
<fieldset>
  <legend>Is your cat an indoor or outdoor cat?</legend>
  <label><input id="indoor" type="radio" name="indoor-outdoor" value="indoor" checked> Indoor</label>
  <label><input id="outdoor" type="radio" name="indoor-outdoor" value="outdoor" > Outdoor</label>
</fieldset>
<fieldset>
  <legend>What's your cat's personality?</legend>
  <input id="loving" type="checkbox" name="personality" value="loving" checked> <label for="loving"> Loving</label>
  <input id="lazy" type="checkbox" name="personality" value="lazy"> <label for="lazy">Lazy</label>
  <input id="energetic" type="checkbox" name="personality" value="energetic"> <label for="energetic"> Energetic</label>
</fieldset>
```
## **Step 62**
Now you will add a footer section to the page.<br>

After the `main` element, add a `footer` element.

```html
</main>
    <footer>
      
    </footer>
```
## **Step 63**
Nest a `p` element with the text `No Copyright - freeCodeCamp.org` within the `footer` element.

```html
<footer>
  <p>No Copyright - freeCodeCamp.org</p>
</footer>
```
## **Step 64**
Make the text `freeCodeCamp.org` into a link by enclosing it in an anchor (`a`) element. The `href` attribute should be set to `https://www.freecodecamp.org`.

```html
<p>
  No Copyright - <a href="https://www.freecodecamp.org"> freeCodeCamp.org</a>
</p>
```
## **Step 65**
Notice that everything you've added to the page so far is inside the` body` element. <br>
All page content elements that should be rendered to the page go inside the `body` element. However, other important information goes inside the `head` element.<br>

Add a `head` element just above the `body` element.

```html
<head>

</head>
<body>
```
## **Step 66**
The `title` element determines what browsers show in the title bar or tab for the page.<br>

Add a `title` element within the` head` element using the text below:<br>

`CatPhotoApp`

```html
<head>
  <title>CatPhotoApp</title>
</head>
```
## **Step 67**
Notice that the entire contents of the page are nested within an `html` element. All other elements must be descendants of this `html` element.<br>

Add the `lang` attribute with the value `en` to the opening `html` tag to specify that the language of the page is English.

```html
<html lang="en">
```
## **Step 68**
All pages should begin with `<!DOCTYPE html>`. This special string is known as a declaration and ensures the browser tries to meet industry-wide specifications.<br>

Add this declaration as the first line of the code.

```html
<!DOCTYPE html>
<html lang="en">
  <head>
  </head>
  <body>
  </body>
</html>

```
## **Step 69**
One more thing. You should allow people to use their native language. <br>
Tell the browser to encode multiple languages by adding a `meta` element as a child of the `head` element. <br>
Set its `charset` attribute to `UTF-8`.

```html
<head>
  <meta charset="UTF-8"></meta>
  <title>CatPhotoApp</title>
</head>
```