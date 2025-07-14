

- UIKit
-  UIEditMenuArrowDirection 

Enumeration

# UIEditMenuArrowDirection

Constants that describe the direction the arrow of the edit menu is pointing.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+visionOS 1.0+

``` source
enum UIEditMenuArrowDirection
```

## Topics

### Constants

case automatic

The arrow is pointing up or down at the object of focus, based on its location in the screen, which is the default.

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

### Configuring the menu

var preferredArrowDirection: UIEditMenuArrowDirection

The preferred direction the arrow of the edit menu is pointing.

var sourcePoint: CGPoint

The source location of the interaction.

