

- WebKit JS
- WebKitAnimationEvent
-  elapsedTime 

Instance Property

# elapsedTime

The duration of the animation, in seconds, since this event was sent, excluding any time the animation is paused. This value is not affected by the value of the CSS -webkit-animation-delay property. If the type of the event is `webkitAnimationStart`, `elapsedTime` is `0`.

Safari Desktop 4.0+Safari Mobile 2.0+

``` source
readonly attribute double elapsedTime;
```

## See Also

### Accessing Properties

animationName

The name of the animation. The value of the CSS -webkit-animation-name property of the animation that caused the event.

