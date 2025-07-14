

- UIKit
- UICellAccessory
-  multiselect(displayed:options:) 

Type Method

# multiselect(displayed:options:)

Creates a multiselect system accessory with the specified display state and configuration options.

iOS 14.0+iPadOS 14.0+Mac CatalysttvOS 14.0+visionOS

``` source
static func multiselect(
    displayed: UICellAccessory.DisplayedState = .whenEditing,
    options: UICellAccessory.MultiselectOptions = MultiselectOptions()
) -> UICellAccessory
```

## Parameters 

`displayed`  

The cell-editing states that the multiselect accessory appears in. This parameter has a default value of UICellAccessory.DisplayedState.whenEditing.

`options`  

Configuration options for the multiselect accessory. See UICellAccessory.MultiselectOptions for possible configuration options.

## Return Value

A configured multiselect cell accessory that changes apperance according to the cell’s selection state. The accessory displays as an empty circle for an unselected cell and as a filled circle with a checkmark for a selected cell. This accessory appears on the leading edge of the cell.

## See Also

### Creating a multiselect accessory

struct MultiselectOptions

Configuration options for a multiselect accessory.

