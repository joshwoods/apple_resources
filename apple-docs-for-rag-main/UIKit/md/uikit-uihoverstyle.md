

- UIKit
-  UIHoverStyle 

Class

# UIHoverStyle

The hover style to apply to a view, including an effect and a shape to use for displaying that effect.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+visionOS 1.0+

``` source
@MainActor
class UIHoverStyle
```

## Topics

### Creating a hover style

convenience init(effect: some UIHoverEffect, shape: UIShape?)

Creates a hover style with the provided effect and shape.

convenience init(shape: UIShape?)

Creates a hover style with the provided shape and an automatic hover effect.

### Specifying a hover shape

var shape: UIShape?

The shape to use for the hover effect.

struct UIShape

An abstract representation of a shape.

### Specifying a hover effect

var effect: any UIHoverEffect

The effect to apply to the view with this style.

struct UIHoverAutomaticEffect

A system-default hover effect that automatically selects the appropriate effect based on the view to which it applies.

struct UIHoverHighlightEffect

An effect that applies a highlight to the view on hover.

struct UIHoverLiftEffect

An effect that can visually lift the view on hover where appropriate.

protocol UIHoverEffect

A hover effect that can apply to a view through a hover style.

### Managing the state of the hover effect

var isEnabled: Bool

A Boolean value that determines whether the hover effect is active.

## Relationships

### Inherits From

- NSObject

### Inherited By

- UIPointerStyle

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCopying
- NSObjectProtocol

## See Also

### Managing the hover appearance

var hoverStyle: UIHoverStyle?

The hover style for the view.

class UIHoverEffectLayer

