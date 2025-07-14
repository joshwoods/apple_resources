

- UIKit
- UIEditMenuConfiguration
-  sourcePoint 

Instance Property

# sourcePoint

The source location of the interaction.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+visionOS 1.0+

``` source
@MainActor
var sourcePoint: CGPoint { get }
```

## Discussion

The system derives the suggested actions list from this point in the interaction’s view. By default, the menu also presents from this location. You can change the presentation source of the menu by implementing the delegate method editMenuInteraction(_:targetRectFor:).

## See Also

### Configuring the menu

var preferredArrowDirection: UIEditMenuArrowDirection

The preferred direction the arrow of the edit menu is pointing.

enum UIEditMenuArrowDirection

Constants that describe the direction the arrow of the edit menu is pointing.

