

- AppKit
- NSAnimation
-  init(duration:animationCurve:) 

Initializer

# init(duration:animationCurve:)

Returns an `NSAnimation` object initialized with the specified duration and animation-curve values.

macOS

``` source
init(
    duration: TimeInterval,
    animationCurve: NSAnimation.Curve
)
```

## Parameters 

`duration`  

The number of seconds over which the animation occurs. Specifying a negative number raises an exception.

`animationCurve`  

An `NSAnimationCurve` constant that describes the relative speed of the animation over its course; if it is zero, the default curve (`NSAnimationEaseInOut`) is used.

## Return Value

An initialized `NSAnimation` instance. Returns `nil` if the object could not be initialized.

## Discussion

You can always later change the duration of an `NSAnimation` object by changing the duration property, even while the animation is running. See “Constants” for descriptions of the NSAnimationCurve constants.

## See Also

### Related Documentation

Cocoa Drawing Guide

Animation Programming Guide for Cocoa

