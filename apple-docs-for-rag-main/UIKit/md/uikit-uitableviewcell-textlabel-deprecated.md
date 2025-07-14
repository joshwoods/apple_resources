

- UIKit
- UITableViewCell
-  textLabel Deprecated

Instance Property

# textLabel

The label to use for the main textual content of the table cell.

iOS 3.0–18.4DeprecatediPadOS 3.0–18.4DeprecatedMac Catalyst 13.1+tvOSvisionOS 1.0–2.4Deprecated

``` source
@MainActor
var textLabel: UILabel? { get }
```

Deprecated

Use a content configuration to manage the cell’s text instead. Use defaultContentConfiguration() to get a default list content configuration, set your primary text to the text property of the configuration, and apply the configuration by setting it to the contentConfiguration property of the cell.

## Mentioned in 

Filling a table with data

Configuring the cells for your table

## Discussion

This property holds the main label of the cell. UITableViewCell adds an appropriate label when you create the cell in a particular cell style. See UITableViewCell.CellStyle for descriptions of the main label in currently defined cell styles.

This property is mutually exclusive with a content configuration. Setting a non-`nil` value for contentConfiguration resets this property to `nil`.

## See Also

### Related Documentation

init(style: UITableViewCell.CellStyle, reuseIdentifier: String?)

Initializes a table cell with a style and a reuse identifier and returns it to the caller.

### Deprecated

var detailTextLabel: UILabel?

The secondary label of the table cell, if one exists.

Deprecated

var imageView: UIImageView?

The image view of the table cell.

Deprecated

