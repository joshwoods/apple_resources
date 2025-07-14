

- UIKit
-  UITableViewFocusUpdateContext 

Class

# UITableViewFocusUpdateContext

A context object that provides information relevant to a specific focus update from one view to another.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+

``` source
@MainActor
class UITableViewFocusUpdateContext
```

## Overview

A focus update context provides extra information that’s only relevant to focus updates involving table views. Instances of this class are ephemeral and are usually discarded after the update is finished.

## Topics

### Locating focusable items in a table view

var previouslyFocusedIndexPath: IndexPath?

Returns the index path of the cell containing the context’s previously focused view.

var nextFocusedIndexPath: IndexPath?

Returns the index path of the cell containing the context’s next focused view.

## Relationships

### Inherits From

- UIFocusUpdateContext

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol
- Sendable

## See Also

### Table management

Estimating the height of a table’s scrolling area

Provide height estimates for your table view’s headers, footers, and rows to ensure that scrolling accurately reflects the size of your content.

class UITableViewController

A view controller that specializes in managing a table view.

protocol UITableViewDelegate

Methods for managing selections, configuring section headers and footers, deleting and reordering cells, and performing other actions in a table view.

