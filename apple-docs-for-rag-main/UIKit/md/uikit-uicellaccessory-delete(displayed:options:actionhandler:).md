

- UIKit
- UICellAccessory
-  delete(displayed:options:actionHandler:) 

Type Method

# delete(displayed:options:actionHandler:)

Creates a delete system accessory with the specified display state, configuration options, and optional action handler.

iOS 14.0+iPadOS 14.0+Mac CatalysttvOS 14.0+visionOS

``` source
static func delete(
    displayed: UICellAccessory.DisplayedState = .whenEditing,
    options: UICellAccessory.DeleteOptions = DeleteOptions(),
    actionHandler: UICellAccessory.ActionHandler? = nil
) -> UICellAccessory
```

## Parameters 

`displayed`  

The cell-editing states that the delete accessory appears in. This parameter has a default value of UICellAccessory.DisplayedState.whenEditing.

`options`  

Configuration options for the delete accessory. See UICellAccessory.DeleteOptions for possible configuration options.

`actionHandler`  

An optional closure that the system calls when a user interacts with the delete accessory.

## Return Value

A configured delete cell accessory. This accessory is a minus sign inside of a circle with the default system red color. This accessory appears on the leading edge of the cell.

## See Also

### Creating a delete accessory

struct DeleteOptions

Configuration options for a delete accessory.

