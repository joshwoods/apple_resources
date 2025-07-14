

- UIKit
- UITableViewCell
-  contentView 

Instance Property

# contentView

The content view of the cell object.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var contentView: UIView { get }
```

## Discussion

The content view of a UITableViewCell object is the default superview for content that the cell displays. If you want to customize cells by simply adding additional views, you should add them to the content view so they position appropriately as the cell transitions in to and out of editing mode.

## See Also

### Related Documentation

var backgroundView: UIView?

The view to use as the background of the cell.

### Managing the content

func defaultContentConfiguration() -> UIListContentConfiguration

Retrieves a default list content configuration for the cell’s style.

var contentConfiguration: (any UIContentConfiguration)?

The current content configuration of the cell.

var automaticallyUpdatesContentConfiguration: Bool

A Boolean value that determines whether the cell automatically updates its content configuration when its state changes.

