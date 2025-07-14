

- UIKit
- UITableViewRowAction
-  backgroundColor Deprecated

Instance Property

# backgroundColor

The background color of the action button.

iOS 8.0–13.0DeprecatediPadOS 8.0–13.0DeprecatedMac Catalyst 13.1–13.1Deprecated

``` source
@NSCopying @MainActor
var backgroundColor: UIColor? { get set }
```

## Discussion

Use this property to specify the background color for your button. If you don’t specify a value for this property, UIKit assigns a default color based on the value in the style property.

## See Also

### Configuring the action’s appearance

var style: UITableViewRowAction.Style

The style applied to the action button.

Deprecated

enum Style

Constants that specify the appearance of action buttons.

Deprecated

var title: String?

The title of the action button.

Deprecated

var backgroundEffect: UIVisualEffect?

The visual effect to apply to the button.

Deprecated

