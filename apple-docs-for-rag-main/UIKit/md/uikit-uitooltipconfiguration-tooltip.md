

- UIKit
- UIToolTipConfiguration
-  toolTip 

Instance Property

# toolTip

The text to display in the tooltip.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+visionOS 1.0+

``` source
@MainActor
var toolTip: String { get }
```

## Discussion

To set the tooltip text, create a tooltip configuration object using either the init(toolTip:) or init(toolTip:in:) methods.

## See Also

### Accessing the configuration settings

var sourceRect: CGRect?

The region of the view or control where the pointer must hover to trigger the appearance of the tooltip.

