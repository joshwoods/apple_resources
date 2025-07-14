

- UIKit
- UITableViewCell
-  imageView Deprecated

Instance Property

# imageView

The image view of the table cell.

iOS 3.0–18.4DeprecatediPadOS 3.0–18.4DeprecatedMac Catalyst 13.1+tvOSvisionOS 1.0–2.4Deprecated

``` source
@MainActor
var imageView: UIImageView? { get }
```

Deprecated

Use a content configuration to manage the cell’s image instead. Use defaultContentConfiguration() to get a default list content configuration, set your image to the image property of the configuration, and apply the configuration by setting it to the contentConfiguration property of the cell.

## Mentioned in 

Configuring the cells for your table

## Discussion

Returns the image view (UIImageView object) of the table view, which initially has no image set. If an image is set, it appears on the left side of the cell, before any label. `UITableViewCell` creates the image-view object when you create the cell.

This property is mutually exclusive with a content configuration. Setting a non-`nil` value for contentConfiguration resets this property to `nil`.

## See Also

### Related Documentation

init(style: UITableViewCell.CellStyle, reuseIdentifier: String?)

Initializes a table cell with a style and a reuse identifier and returns it to the caller.

### Deprecated

var textLabel: UILabel?

The label to use for the main textual content of the table cell.

Deprecated

var detailTextLabel: UILabel?

The secondary label of the table cell, if one exists.

Deprecated

