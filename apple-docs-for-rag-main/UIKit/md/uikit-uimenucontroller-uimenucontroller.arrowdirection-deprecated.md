

- UIKit
- UIMenuController
-  UIMenuController.ArrowDirection Deprecated

Enumeration

# UIMenuController.ArrowDirection

The direction the arrow of the editing menu is pointing.

iOS 3.2–16.0DeprecatediPadOS 3.2–16.0DeprecatedMac Catalyst 13.1–16.0DeprecatedvisionOS 1.0–1.0Deprecated

``` source
enum ArrowDirection
```

## Topics

### Constants

case `default`

The arrow is pointing up or down at the object of focus based on its location in the screen.

case up

The arrow is pointing up at the object of focus.

case down

The arrow is pointing down at the object of focus.

case left

The arrow is pointing left at the object of focus.

case right

The arrow is pointing right at the object of focus.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Positioning the menu

var menuFrame: CGRect

Returns the frame of the editing menu.

Deprecated

var arrowDirection: UIMenuController.ArrowDirection

The direction the arrow of the editing menu is pointing.

Deprecated

func setTargetRect(CGRect, in: UIView)

Sets the area in a view above or below which the editing menu is positioned.

Deprecated

