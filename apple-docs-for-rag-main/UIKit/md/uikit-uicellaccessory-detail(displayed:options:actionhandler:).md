

- UIKit
- UICellAccessory
-  detail(displayed:options:actionHandler:) 

Type Method

# detail(displayed:options:actionHandler:)

Creates a detail system accessory with the specified display state, configuration options, and optional action handler.

iOS 15.4+iPadOS 15.4+Mac CatalysttvOS 15.4+visionOS

``` source
static func detail(
    displayed: UICellAccessory.DisplayedState = .always,
    options: UICellAccessory.DetailOptions = DetailOptions(),
    actionHandler: UICellAccessory.ActionHandler? = nil
) -> UICellAccessory
```

## Parameters 

`displayed`  

The cell-editing states that the detail accessory appears in. This parameter has a default value of UICellAccessory.DisplayedState.always.

`options`  

Configuration options for the detail accessory. See UICellAccessory.DetailOptions for possible configuration options.

`actionHandler`  

An optional closure that the system calls when a user interacts with the detail accessory.

## Return Value

A configured detail cell accessory. The accessory displays as the system information button. This accessory appears on the trailing edge of the cell.

## See Also

### Creating a detail accessory

struct DetailOptions

Configuration options for a detail accessory.

