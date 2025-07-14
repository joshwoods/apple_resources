

- UIKit
- UIToolTipConfiguration
-  sourceRect 

Instance Property

# sourceRect

The region of the view or control where the pointer must hover to trigger the appearance of the tooltip.

iOS 15.0+iPadOS 15.0+Mac CatalystvisionOS

``` source
@MainActor @preconcurrency
var sourceRect: CGRect? { get }
```

## Discussion

To set sourceRect, create a tooltip configuration object using the init(toolTip:in:) method.

## See Also

### Accessing the configuration settings

var toolTip: String

The text to display in the tooltip.

