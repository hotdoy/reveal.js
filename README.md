# reveal.js

Reveal content as it enter the viewport using intersection observer.

## Usage

### Add the script

```<script src="/user/themes/hotdoy/js/reveal.js"></script>```

### Add reveal effect to an element.

Add ```data-reveal``` to any element to trigger the default reveal animation (fade in).  

You can add any custom classes you want to overwrite the default animation. ```data-reveal="myClass yetAnother"```.

the class ```unrevealed``` will be added to all elements not in the viewport when the page load. Any element that ARE in the viewport will be let unafected.

If you want to animate any elements visible in the viewport on page load, you can add ```data-reveal-initialdelay``` anywhere in the page whit any value you might want (in ms) ex: ```data-reveal-initialdelay="800"```.
