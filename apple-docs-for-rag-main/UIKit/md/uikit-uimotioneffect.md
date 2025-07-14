

- UIKit
-  UIMotionEffect 

Class

# UIMotionEffect

An abstract superclass for defining motion-based modifiers for views.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
class UIMotionEffect
```

## Overview

Subclasses of UIMotionEffect are responsible for defining the behavior to apply to a view when motion is detected. They do this by overriding the keyPathsAndRelativeValues(forViewerOffset:) method and returning one or more key paths representing the view properties to modify.

### Subclassing notes

This class is abstract and can’t be instantiated directly. You can use the UIInterpolatingMotionEffect class to implement effects or you can subclass and implement your own effects. If you subclass, your subclass must conform to the NSCopying and NSCoding protocols and must implement the keyPathsAndRelativeValues(forViewerOffset:) method.

## Topics

### Initializing a motion effect

init()

Initializes the motion effect to its default state.

init?(coder: NSCoder)

Creates a motion effect from data in an unarchiver.

### Getting the key paths

func keyPathsAndRelativeValues(forViewerOffset: UIOffset) -> [String : Any]?

For a given set of offset values, returns the view properties (and corresponding values) to update.

## Relationships

### Inherits From

- NSObject

### Inherited By

- UIInterpolatingMotionEffect
- UIMotionEffectGroup

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

