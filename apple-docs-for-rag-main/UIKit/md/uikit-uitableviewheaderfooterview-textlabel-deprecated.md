

- UIKit
- UITableViewHeaderFooterView
-  textLabel Deprecated

Instance Property

# textLabel

A primary text label for the view.

iOS 6.0–18.4DeprecatediPadOS 6.0–18.4DeprecatedMac Catalyst 13.1+tvOSvisionOS 1.0–2.4Deprecated

``` source
@MainActor
var textLabel: UILabel? { get }
```

Deprecated

Use a content configuration to manage the view’s text instead. Use defaultContentConfiguration() to get a default list content configuration, set your primary text to the text property of the configuration, and apply the configuration by setting it to the contentConfiguration property of the view.

## Discussion

Accessing the value in this property causes the view to create a default label for displaying a detail text string. If you are managing the content of the view yourself by adding subviews to the contentView property, you should not access this property.

The label sizes to fit the content view area in the best way possible according to the size of the string. Its size also adjusts depending on whether there is a detail text label present.

This property is mutually exclusive with a content configuration. Setting a non-`nil` value for contentConfiguration resets this property to `nil`.

## See Also

### Deprecated

var detailTextLabel: UILabel?

A detail text label for the view.

Deprecated

