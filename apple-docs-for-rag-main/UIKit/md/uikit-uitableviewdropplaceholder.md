

- UIKit
-  UITableViewDropPlaceholder 

Class

# UITableViewDropPlaceholder

A placeholder cell that supports customizing the drop preview parameters.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
class UITableViewDropPlaceholder
```

## Overview

When you want to insert a placeholder cell into your table, create a UITableViewDropPlaceholder object and pass it to the drop(_:to:) method of your UITableViewDropCoordinator. You use a placeholder cell to display a temporary interface while you load the cell’s contents asynchronously. For example, your placeholder cell might display a progress indicator or a message that the cell content isn’t yet available. The placeholder object contains the reuse identifier of the temporary cell you want to display in your table. It can also include a custom preview to use during the drop.

You must register the cells you use with your placeholders in advance. In your storyboard file, add a table view cell object to your table, configure its appearance, set its class to UITableViewCell (or an appropriate subclass), and assign a reuse identifier to it. When you create your UITableViewDropPlaceholder object, pass the cell’s reuse identifier to init(insertionIndexPath:reuseIdentifier:rowHeight:). The table view uses the information in your placeholder object to insert the cell into the table.

Set the cellUpdateHandler to a block of code that configures the cell as a placeholder for the incoming data.

For more information, see Supporting drag and drop in table views.

Important

Placeholder cells are meant to be a temporary part of your table view. Always replace them with actual cells as soon as possible, or cancel the drop to remove them from the table. Use the methods of a UITableViewDropPlaceholderContext object to remove placeholders from your table.

## Topics

### Providing preview parameters

var previewParametersProvider: ((UITableViewCell) -> UIDragPreviewParameters?)?

The handler block that provides the preview parameters for the specified cell.

## Relationships

### Inherits From

- UITableViewPlaceholder

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Placeholder cells

protocol UITableViewDropPlaceholderContext

An object for tracking a placeholder cell that you added to your table during a drop operation.

class UITableViewPlaceholder

An object that contains information about a placeholder cell being inserted into a table.

