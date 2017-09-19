# spotter
Interact with elements when they enter or exit view

```javascript
var spotter = new Spotter();

spotter
  .add('.element', {
    animation: 'fadeIn',  // Can be string of class or object with CSS animation properties.
    hide: true, // Can be boolean or string of class that is set on the element.
    repeat: true, // Boolean. Hides elements again when out of view.
    lazyLoad: true, // Boolean. Lazy loads img elements with a data-src attribute.
    spotted: (element) => { // Returns the element that is spotted when in viewport
      console.log(element);
    },
    unSpotted: (element) => { // Returns the element that is unspotted when is out of viewport.
      console.log(element);
    }
  });
```
