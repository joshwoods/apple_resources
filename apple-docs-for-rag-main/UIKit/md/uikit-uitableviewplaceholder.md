

- UIKit
-  UITableViewPlaceholder 

Class

# UITableViewPlaceholder

An object that contains information about a placeholder cell being inserted into a table.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
class UITableViewPlaceholder
```

## Overview

During a drop operation, create a UITableViewDropPlaceholder object (instead of this one) to insert placeholders into your table.

## Topics

### Creating a placeholder cell

init(insertionIndexPath: IndexPath, reuseIdentifier: String, rowHeight: CGFloat)

Creates a placeholder object with the specified index path and cell-related information.

### Updating the cell’s content

var cellUpdateHandler: ((UITableViewCell) -> Void)?

The block that updates the contents of the placeholder cell.

## Relationships

### Inherits From

- NSObject

### Inherited By

- UITableViewDropPlaceholder

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol
- Sendable

## See Also

### Placeholder cells

protocol UITableViewDropPlaceholderContext

An object for tracking a placeholder cell that you added to your table during a drop operation.

class UITableViewDropPlaceholder

A placeholder cell that supports customizing the drop preview parameters.

