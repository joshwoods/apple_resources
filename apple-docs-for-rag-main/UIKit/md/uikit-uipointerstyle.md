

- UIKit
-  UIPointerStyle 

Class

# UIPointerStyle

An object that defines the pointer shape and effect.

iOS 13.4+iPadOS 13.4+Mac Catalyst 13.4+visionOS 1.0+

``` source
@MainActor
class UIPointerStyle
```

## Overview

Whenever possible, match pointer styles to UIKit styles and make them consistent with the visual intent of similar views.

Note

When supporting the use of Apple Pencil, effect-based styles, such as a pointer style created using init(effect:shape:) are fully supported, but shape-based pointer styles created using init(shape:constrainedAxes:) aren’t.

For more information, see Human Interface Guidelines.

## Topics

### Creating a pointer style

convenience init(effect: UIPointerEffect, shape: UIPointerShape?)

Applies the provided content effect and pointer shape to the current region.

convenience init(shape: UIPointerShape, constrainedAxes: UIAxis)

Morphs the pointer into the provided shape when hovering over the current region.

class func hidden() -> Self

Hides the pointer when it moves over the current region.

class func system() -> Self

Morphs the pointer into a default system-style pointer.

### Specifying pointer accessories

var accessories: [UIPointerAccessory]

Accessories to display alongside the pointer.

class UIPointerAccessory

Constants that describe accessories to display alongside the primary pointer.

## Relationships

### Inherits From

- UIHoverStyle

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCopying
- NSObjectProtocol

## See Also

### Pointer styles

enum UIPointerShape

An object that defines the shape of custom pointers.

enum UIPointerEffect

An effect that alters a view’s appearance when a pointer enters the current region.

class UIPointerAccessory

Constants that describe accessories to display alongside the primary pointer.

