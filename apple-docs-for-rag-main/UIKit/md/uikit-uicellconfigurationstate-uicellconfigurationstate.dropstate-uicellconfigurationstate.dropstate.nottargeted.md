

- UIKit
- UICellConfigurationState
- UICellConfigurationState.DropState
-  UICellConfigurationState.DropState.notTargeted 

Case

# UICellConfigurationState.DropState.notTargeted

A drag session is active and can perform a drop in the cell’s container, but the cell itself isn’t the drop target.

iOS 14.0+iPadOS 14.0+Mac CatalysttvOS 14.0+visionOS

``` source
case notTargeted
```

## See Also

### Drop states

case none

The system hasn’t associated the cell with a drag session.

case targeted

The cell is the drop target for a drag session.

