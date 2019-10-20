# reveal.js

Reveal content as it enter the viewport using intersection observer.

## Usage

### Add the script

```<script src="/user/themes/hotdoy/js/reveal.js"></script>```

### Add reveal effect to an element.

Add ```data-reveal``` to any element to trigger the default reveal animation (fade in).  

You can add any custom classes you want to overwrite the default animation. ```data-reveal="myClass yetAnother"```.

the class ```unrevealed``` will be added to all elements outside of the viewport when the page load. Any element that ARE in the viewport will be let unafected.

If you want to animate elements visible in the viewport on page load, you can add ```data-reveal-initialdelay``` anywhere in the page with value in ms. ex: ```data-reveal-initialdelay="800"```. This is mostly useful if you have some kind of loader.

Jquery is needed only for ```$(init)```.
