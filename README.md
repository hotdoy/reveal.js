# reveal.js

Reveal elements as they enter the viewport using intersection observer and CSS.

## Usage

### Add the script

```<script src="/path/reveal.js"></script>```

### Add reveal effect to an element.

Add ```data-reveal``` to an element. 
That's it!

ex: ```<div data-reveal>What a nice day!</div>```

You can add your own reveal animation by simply creating new css classes and animations.

ex: ```<div data-reveal="myOwnClass">What a nice day!</div>```

### Apply reveal animation to all child element.

Adding ```data-auto-reveal``` on a parent element will automatically add the ```data-reveal``` attribute with the related classes to all it's childrens.

### Delaying the initial reveal 

You can delay the whole process by adding ```data-reveal-delay``` on the body element of a page (Or any element really. Only the first found value will be used.)
