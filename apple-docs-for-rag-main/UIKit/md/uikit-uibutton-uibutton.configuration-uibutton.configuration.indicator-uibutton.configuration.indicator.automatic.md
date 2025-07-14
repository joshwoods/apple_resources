

- UIKit
- UIButton
- UIButton.Configuration
- UIButton.Configuration.Indicator
-  UIButton.Configuration.Indicator.automatic 

Case

# UIButton.Configuration.Indicator.automatic

A constant that automatically determines an indicator style according to the button’s properties.

iOS 16.0+iPadOS 16.0+Mac CatalysttvOS 16.0+visionOS

``` source
case automatic
```

## Discussion

With this behavior, the system automatically shows an indicator if the button shows a menu and has single-selection behavior (when its isContextMenuInteractionEnabled, showsMenuAsPrimaryAction, and changesSelectionAsPrimaryAction properties are true).

## See Also

### Indicator styles

case none

A constant that doesn’t show an indicator.

case popup

A constant that shows a popup-style indicator.

