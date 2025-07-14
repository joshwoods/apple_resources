

- UIKit
- UIEditMenuConfiguration
-  preferredArrowDirection 

Instance Property

# preferredArrowDirection

The preferred direction the arrow of the edit menu is pointing.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+visionOS 1.0+

``` source
@MainActor
var preferredArrowDirection: UIEditMenuArrowDirection { get set }
```

## Discussion

The default, UIEditMenuArrowDirection.automatic, is an arrow pointing up or down at the object of focus, based on its location in the screen.

## See Also

### Configuring the menu

enum UIEditMenuArrowDirection

Constants that describe the direction the arrow of the edit menu is pointing.

var sourcePoint: CGPoint

The source location of the interaction.

