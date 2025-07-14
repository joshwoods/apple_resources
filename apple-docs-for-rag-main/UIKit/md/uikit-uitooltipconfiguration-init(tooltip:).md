

- UIKit
- UIToolTipConfiguration
-  init(toolTip:) 

Initializer

# init(toolTip:)

Creates a tooltip configuration and sets the tooltip text.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+visionOS 1.0+

``` source
@MainActor
convenience init(toolTip: String)
```

## Parameters 

`toolTip`  

The text that appears in the tooltip.

## Discussion

Create a configuration using this method to show the tooltip when the pointer hovers over any area of the view or control. For example, the following code listing creates a configuration that instructs the view to show the tooltip when the pointer hovers over any area of the view:

```
let configuration = UIToolTipConfiguration(toolTip: "The color is \(colorName).")
```

## See Also

### Creating a tooltip configuration

convenience init(toolTip: String, in: CGRect)

Creates a tooltip configuration, and sets the tooltip text and hover region within the view or control.

