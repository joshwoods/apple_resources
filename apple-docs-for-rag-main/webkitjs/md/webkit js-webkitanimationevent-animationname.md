

- WebKit JS
- WebKitAnimationEvent
-  animationName 

Instance Property

# animationName

The name of the animation. The value of the CSS -webkit-animation-name property of the animation that caused the event.

Safari Desktop 10.0+Safari Mobile 10.0+

``` source
readonly attribute DOMString animationName;
```

## See Also

### Accessing Properties

elapsedTime

The duration of the animation, in seconds, since this event was sent, excluding any time the animation is paused. This value is not affected by the value of the CSS -webkit-animation-delay property. If the type of the event is `webkitAnimationStart`, `elapsedTime` is `0`.

### Related Documentation

Safari CSS Visual Effects Guide

