

- UIKit
-  UIMotionEffectGroup 

Class

# UIMotionEffectGroup

A collection of motion effects that you want to apply to a view at the same time.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
class UIMotionEffectGroup
```

## Overview

This class behaves similarly to the CAAnimationGroup class in Core Animation. The key paths and values returned by each motion effect object are applied simultaneously and with the same timing. Because UIMotionEffectGroup is a subclass of UIMotionEffect, you can treat it like a single motion effect in your code. After setting a value for the motionEffects property, add the group object to one or more of your views.

## Topics

### Setting the group items

var motionEffects: [UIMotionEffect]?

An array of motion effect objects to apply as a group to the view.

## Relationships

### Inherits From

- UIMotionEffect

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSCopying
- NSObjectProtocol
- Sendable

## See Also

### View-based effects

class UIInterpolatingMotionEffect

An object that maps the horizontal or vertical tilt of a device to values that you specify so that UIKit can apply those values to your views.

