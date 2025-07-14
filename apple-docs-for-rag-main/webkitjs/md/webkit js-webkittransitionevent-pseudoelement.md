

- WebKit JS
- WebKitTransitionEvent
-  pseudoElement 

Instance Property

# pseudoElement

An abstract element representing the portion of the CSS render tree on which the transition occurs.

Safari Desktop 10.0+Safari Mobile 10.0+

``` source
readonly attribute DOMString pseudoElement;
```

## Discussion

This element is an empty string if the transition occurs on a non-abstract element.

