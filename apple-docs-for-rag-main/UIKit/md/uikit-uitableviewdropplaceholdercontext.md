

- UIKit
-  UITableViewDropPlaceholderContext 

Protocol

# UITableViewDropPlaceholderContext

An object for tracking a placeholder cell that you added to your table during a drop operation.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
protocol UITableViewDropPlaceholderContext : UIDragAnimating
```

## Overview

Don’t create instances of this class yourself. Instead, call drop(_:to:) from your drop coordinator object. That method inserts a placeholder cell into the table and returns a UITableViewDropPlaceholderContext object for managing that placeholder.

When you’re ready to swap a placeholder cell for a cell with the actual data, call the commitInsertion(dataSourceUpdates:) method of the context object. To remove the placeholder cell without providing a replacement, call deletePlaceholder() instead.

## Topics

### Updating the placeholder cell

func commitInsertion(dataSourceUpdates: (IndexPath) -> Void) -> Bool

Exchanges the placeholder cell for a cell with the final content.

**Required**

### Removing the placeholder cell

func deletePlaceholder() -> Bool

Removes an unneeded placeholder cell from the table view.

**Required**

### Getting the drag item

var dragItem: UIDragItem

The drag item represented by the placeholder cell.

**Required**

## Relationships

### Inherits From

- NSObjectProtocol
- UIDragAnimating

## See Also

### Placeholder cells

class UITableViewDropPlaceholder

A placeholder cell that supports customizing the drop preview parameters.

class UITableViewPlaceholder

An object that contains information about a placeholder cell being inserted into a table.

