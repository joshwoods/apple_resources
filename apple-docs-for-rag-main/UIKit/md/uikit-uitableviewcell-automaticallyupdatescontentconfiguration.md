

- UIKit
- UITableViewCell
-  automaticallyUpdatesContentConfiguration 

Instance Property

# automaticallyUpdatesContentConfiguration

A Boolean value that determines whether the cell automatically updates its content configuration when its state changes.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+tvOS 14.0+visionOS 1.0+

``` source
@MainActor
var automaticallyUpdatesContentConfiguration: Bool { get set }
```

## Discussion

When this value is true, the cell automatically calls updated(for:) on its contentConfiguration when the cell’s configurationState changes, and applies the updated configuration back to the cell. The default value is true.

If you override updateConfiguration(using:) to manually update and customize the content configuration, disable automatic updates by setting this property to false.

## See Also

### Managing the content

func defaultContentConfiguration() -> UIListContentConfiguration

Retrieves a default list content configuration for the cell’s style.

var contentConfiguration: (any UIContentConfiguration)?

The current content configuration of the cell.

var contentView: UIView

The content view of the cell object.

