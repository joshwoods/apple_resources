

- UIKit
-  UIPointerShape 

Enumeration

# UIPointerShape

An object that defines the shape of custom pointers.

iOS 13.4+iPadOS 13.4+Mac CatalystvisionOS

``` source
enum UIPointerShape
```

## Overview

If the desired pointer shape can be expressed as a rounded rectangle, use UIPointerShape.roundedRect(_:radius:) for best results.

## Topics

### Specifying pointer shapes

case horizontalBeam(length: CGFloat)

The pointer morphs into a horizontal beam using the specified length.

case verticalBeam(length: CGFloat)

The pointer morphs into a vertical beam using the specified length.

case path(UIBezierPath)

The pointer morphs into the given Bézier path.

case roundedRect(CGRect, radius: CGFloat)

The pointer morphs into a rounded rectangle using the provided corner radius.

### Accessing corner radius

static let defaultCornerRadius: CGFloat

The default corner radius for a pointer using a rounded rectangle.

## Relationships

### Conforms To

- Copyable

## See Also

### Pointer styles

class UIPointerStyle

An object that defines the pointer shape and effect.

enum UIPointerEffect

An effect that alters a view’s appearance when a pointer enters the current region.

class UIPointerAccessory

Constants that describe accessories to display alongside the primary pointer.

