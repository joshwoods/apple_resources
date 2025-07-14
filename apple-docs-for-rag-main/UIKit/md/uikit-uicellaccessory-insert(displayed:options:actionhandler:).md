

- UIKit
- UICellAccessory
-  insert(displayed:options:actionHandler:) 

Type Method

# insert(displayed:options:actionHandler:)

Creates an insert system accessory with the specified display state, configuration options, and optional action handler.

iOS 14.0+iPadOS 14.0+Mac CatalysttvOS 14.0+visionOS

``` source
static func insert(
    displayed: UICellAccessory.DisplayedState = .whenEditing,
    options: UICellAccessory.InsertOptions = InsertOptions(),
    actionHandler: UICellAccessory.ActionHandler? = nil
) -> UICellAccessory
```

## Parameters 

`displayed`  

The cell-editing states that the insert accessory appears in. This parameter has a default value of UICellAccessory.DisplayedState.whenEditing.

`options`  

Configuration options for the insert accessory. See UICellAccessory.InsertOptions for possible configuration options.

`actionHandler`  

An optional closure that the system calls when a user interacts with the insert accessory.

## Return Value

A configured insert cell accessory. This accessory is a plus sign inside of a circle with the default system green color. This accessory appears on the leading edge of the cell.

## See Also

### Creating an insert accessory

struct InsertOptions

Configuration options for an insert accessory.

