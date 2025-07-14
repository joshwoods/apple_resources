

- UIKit
- UITableViewCell
- UITableViewCell.FocusStyle
-  UITableViewCell.FocusStyle.custom 

Case

# UITableViewCell.FocusStyle.custom

The cell doesn’t alter its appearance automatically when it becomes focused.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+

``` source
case custom
```

## Discussion

Specifying this style allows you to create your own custom appearance for the cell. It’s recommended that you create custom-looking cells by subclassing UITableViewCell and overriding didUpdateFocus(in:with:).

## See Also

### Constants

case `default`

The cell alters its appearance in a standard, system-defined way when it becomes focused.

