

- UIKit
- UICellAccessory
-  checkmark(displayed:options:) 

Type Method

# checkmark(displayed:options:)

Creates a checkmark system accessory with the specified display state and configuration options.

iOS 14.0+iPadOS 14.0+Mac CatalysttvOS 14.0+visionOS

``` source
static func checkmark(
    displayed: UICellAccessory.DisplayedState = .always,
    options: UICellAccessory.CheckmarkOptions = CheckmarkOptions()
) -> UICellAccessory
```

## Parameters 

`displayed`  

The cell-editing states that the checkmark appears in. This parameter has a default value of UICellAccessory.DisplayedState.always.

`options`  

Configuration options for the checkmark. See UICellAccessory.CheckmarkOptions for possible configuration options.

## Return Value

A configured checkmark cell accessory. This accessory is a checkmark with the default system green color. This accessory appears on the trailing edge of the cell.

## See Also

### Creating a checkmark accessory

struct CheckmarkOptions

Configuration options for a checkmark accessory.

