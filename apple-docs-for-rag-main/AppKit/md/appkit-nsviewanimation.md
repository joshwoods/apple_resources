

- AppKit
-  NSViewAnimation 

Class

# NSViewAnimation

An animation of an app’s views, limited to changes in frame location and size, and to fade-in and fade-out effects.

macOS

``` source
class NSViewAnimation
```

## Overview

An NSViewAnimation object takes an array of dictionaries from which it determines the objects to animate and the effects to apply to them. Each dictionary must have a target object and, optionally, properties that specify beginning and ending frame and whether to fade in or fade out. (See NSViewAnimation.Key for further information.) Animations with NSViewAnimation are, by default, in non-blocking mode over a duration of 0.5 seconds using the ease in-out animation curve. But you can configure the animation to have any duration, curve, frame rate, and blocking mode. You may also set progress marks, assign a delegate, and implement delegation methods in order to animate view and windows concurrent with the ones specified as targets in the view-animation dictionary.

Invoking the NSAnimation stop() method on a running NSViewAnimation object moves the animation to the end frame.

## Topics

### Initializing an NSViewAnimation object

init(viewAnimations: [[NSViewAnimation.Key : Any]])

Returns an `NSViewAnimation` object initialized with the supplied information.

### Getting and setting view-animation dictionaries

var viewAnimations: [[NSViewAnimation.Key : Any]]

The dictionaries defining the objects to animate.

struct Key

The following string constants are keys for the dictionaries in the array passed into init(viewAnimations:) and viewAnimations.

struct EffectName

The following constants specify the animation effect to apply and are used as values for the animation effect property of the animation view. See the description of effect for usage details.

## Relationships

### Inherits From

- NSAnimation

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSCopying
- NSObjectProtocol

## See Also

### View-Based Animations

protocol NSAnimatablePropertyContainer

A set of methods that defines a way to add animation to an existing class with a minimum of API impact.

class NSAnimationContext

An animation context, which contains information about environment and state.

typealias Progress

The animation progress, as a floating-point number between `0.0` and `1.0`.

enum NSAnimationEffect

The type for standard system animation effects, which include both display and sound.

Deprecated

