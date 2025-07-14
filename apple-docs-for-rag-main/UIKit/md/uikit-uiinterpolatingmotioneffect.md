

- UIKit
-  UIInterpolatingMotionEffect 

Class

# UIInterpolatingMotionEffect

An object that maps the horizontal or vertical tilt of a device to values that you specify so that UIKit can apply those values to your views.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
class UIInterpolatingMotionEffect
```

## Overview

You use this class to determine the amount of tilt along a single axis to apply to a view. After creating an instance of this class, you must assign appropriate values to the minimumRelativeValue and maximumRelativeValue properties. As the user moves the device, the motion effect object translates the fixed offset values returned by the system (which are in the range `-1` to `1`) to the range of values you specified. UIKit then applies the translated values to any target views.

## Topics

### Initializing a motion effect

init(keyPath: String, type: UIInterpolatingMotionEffect.EffectType)

Initializes and returns an interpolating motion effect object configured for the specific tilt direction.

init?(coder: NSCoder)

Creates a motion effect from data in an unarchiver.

### Accessing the motion attributes

var keyPath: String

The key path you want to modify on the view.

var type: UIInterpolatingMotionEffect.EffectType

The tilt direction to monitor.

var minimumRelativeValue: Any?

The value that maps to the minimum viewer offset.

var maximumRelativeValue: Any?

The value that maps to the maximum viewer offset.

### Constants

enum EffectType

The axis to use when interpolating values.

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

## See Also

### View-based effects

class UIMotionEffectGroup

A collection of motion effects that you want to apply to a view at the same time.

