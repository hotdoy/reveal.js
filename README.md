# reveal.js

Reveal elements as they enter the viewport using intersection observer and CSS.

## Usage

### Add related js and css.

```<script src="/path/to/js/reveal.js"></script>```  
```<link href="/path/to/css/reveal.css" type="text/css" rel="stylesheet">```

### Add reveal animation effect to an element.

Simply add ```data-reveal``` to an element. 

ex: ```<div data-reveal>What a nice day!</div>```

You can add your own reveal animation by creating new css classes and animations.

ex: ```<div data-reveal="myOwnClass">What a nice day!</div>```

### Apply reveal animation to children.

Adding ```data-auto-reveal``` on a parent element will automatically add the ```data-reveal``` attribute with related classes to it's children.

### Delaying the initial reveal 

Delay the whole process by adding ```data-reveal-delay="1000"``` (using milliseconds) on any element of your page.
(the body tag could be a good choice. You could also put it on a loader you want to sync the reveal with. We really don't care.)

## Good to know
Since the script runs AFTER everything is loaded, The affected elements are probably going to flash or move around when this thing kicks off.
I suggest using reveal.js in conjunction with loading.js. 
A simple loader that just get the fuck out when done and give you access to simple page state like ```loading```, ```loaded``` and ```unloading``` so you can fake those ajax page transitions like a pro.

And while you're at it. Why not use links.js to manage external and internal links, augment perceived performances using prerender and giving you acces to the ```navigating``` page state.
