# LM Responsive Popup
Responsive popup made with HTML and CSS

### Installation
1. Copy 'style.css' located inside 'styles/css' into your project and link it with ```<link>```.
2. Copy the basic structure from 'popup.html' into your html
3. Copy the JavaScript snippet into your head inside ```<script>``` tags.
4. Enjoy your popup's!

### Customization
I made the css with SCSS and I've created some variables to customize the popup visual aspect.

- ```$maxHeight```: refers to the popup max height. Default is 80%.
- ```$padding```: refers to the popup content padding. Default is 30px.
- ```$primary```: refers to the primary color I've used. Default is #FFFFFF.
- ```$secondary```: refers to the secondary color I've used. Default is #448AFF (blue);

**NOTE**: If you use above variables, you'll need to re-compile the code into CSS.

##### Black background that surrounds the popup
Any popup created is sorrounded by black layer that doesn't allow click below it. You can _disable_ this background
removing this line of HTML:

```html
<div class="popup-background"></div>
```

##### Predefined height and width
You can set custom height and width of the popup simply adding next CSS line to the ```.popup > .popup-container``` class:
```css
height: 500px;
width: 600px; /* Override actual width */
```

With current measures it works well in any device but it's up to you modify them :).

### JavaScript
This popup doesn't need lot of lines of code, one to show the popup and one to close it. In 'popup.html' you can find two 
ways to acomplish that: one using jQuery and other using Vanilla JS.

As you can see, there is a helper class ```.show``` that allows you to show/hide the popup when it's toggled so it's so easy
 to use it with jQuery ```toggleClass()``` method.
 
### License
All content is licensed under GPL v3 so you are free to use this library and all its content in your projects.