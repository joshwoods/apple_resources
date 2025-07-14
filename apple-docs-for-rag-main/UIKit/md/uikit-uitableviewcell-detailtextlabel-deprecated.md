

- UIKit
- UITableViewCell
-  detailTextLabel Deprecated

Instance Property

# detailTextLabel

The secondary label of the table cell, if one exists.

iOS 3.0–18.4DeprecatediPadOS 3.0–18.4DeprecatedMac Catalyst 13.1+tvOSvisionOS 1.0–2.4Deprecated

``` source
@MainActor
var detailTextLabel: UILabel? { get }
```

Deprecated

Use a content configuration to manage the cell’s text instead. Use defaultContentConfiguration() to get a default list content configuration, set your secondary text to the secondaryText property of the configuration, and apply the configuration by setting it to the contentConfiguration property of the cell.

## Mentioned in 

Configuring the cells for your table

## Discussion

Holds the secondary (or detail) label of the cell. `UITableViewCell` adds an appropriate label when you create the cell in a style that supports secondary labels. If the style doesn’t support detail labels, `nil` returns. See UITableViewCell.CellStyle for descriptions of the main label in currently defined cell styles.

This property is mutually exclusive with a content configuration. Setting a non-`nil` value for contentConfiguration resets this property to `nil`.

## See Also

### Related Documentation

init(style: UITableViewCell.CellStyle, reuseIdentifier: String?)

Initializes a table cell with a style and a reuse identifier and returns it to the caller.

### Deprecated

var textLabel: UILabel?

The label to use for the main textual content of the table cell.

Deprecated

var imageView: UIImageView?

The image view of the table cell.

Deprecated

