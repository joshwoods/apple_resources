

- UIKit
- UIButton
- UIButton.Configuration
-  buttonSize 

Instance Property

# buttonSize

A size that requests a preferred size for the button.

iOS 15.0+iPadOS 15.0+Mac CatalysttvOS 15.0+visionOS

``` source
var buttonSize: UIButton.Configuration.Size { get set }
```

## Discussion

The size indicates a system-defined size you prefer for this button. The exact size of the button may change regardless of this value.

## See Also

### Configuring layout

enum Size

A predefined size for button elements.

var contentInsets: NSDirectionalEdgeInsets

The distance from the button’s content area to its bounds.

func setDefaultContentInsets()

Restores the default content insets.

