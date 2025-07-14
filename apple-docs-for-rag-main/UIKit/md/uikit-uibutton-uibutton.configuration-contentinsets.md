

- UIKit
- UIButton
- UIButton.Configuration
-  contentInsets 

Instance Property

# contentInsets

The distance from the button’s content area to its bounds.

iOS 15.0+iPadOS 15.0+Mac CatalysttvOS 15.0+visionOS

``` source
var contentInsets: NSDirectionalEdgeInsets { get set }
```

## Discussion

A button has a default inset based on its styling. This property is an additional inset applied after that default inset.

## See Also

### Configuring layout

var buttonSize: UIButton.Configuration.Size

A size that requests a preferred size for the button.

enum Size

A predefined size for button elements.

func setDefaultContentInsets()

Restores the default content insets.

