

- UIKit
- UICellConfigurationState
- UICellConfigurationState.DropState
-  UICellConfigurationState.DropState.none 

Case

# UICellConfigurationState.DropState.none

The system hasn’t associated the cell with a drag session.

iOS 14.0+iPadOS 14.0+Mac CatalysttvOS 14.0+visionOS

``` source
case none
```

## See Also

### Drop states

case notTargeted

A drag session is active and can perform a drop in the cell’s container, but the cell itself isn’t the drop target.

case targeted

The cell is the drop target for a drag session.

