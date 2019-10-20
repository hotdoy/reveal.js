# reveal.js

Reveal elements as they enter the viewport using intersection observer.

## Usage

### Add the script

```<script src="/path/reveal.js"></script>```

### Add reveal effect to an element.

Add ```data-reveal``` to any element to trigger the default reveal animation (fade in).  
ex: ```<div data-reveal>What a nice day!</div>```

You can add any custom classes you want to overwrite the default animation. ```data-reveal="myClass yetAnother"```.

the class ```unrevealed``` will be added to all elements outside of the viewport when the page load. Any element that ARE in the viewport will be left unafected.

If you want to animate elements visible in the viewport on page load, you can add ```data-reveal-initialdelay``` anywhere in the page with a value in ms. ex: ```data-reveal-initialdelay="800"```. Mostly useful if you have some kind of loader.

### Dependencies
- JQuery
