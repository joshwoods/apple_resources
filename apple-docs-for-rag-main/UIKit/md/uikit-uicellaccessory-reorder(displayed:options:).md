

- UIKit
- UICellAccessory
-  reorder(displayed:options:) 

Type Method

# reorder(displayed:options:)

Creates a reorder system accessory with the specified display state and configuration options.

iOS 14.0+iPadOS 14.0+Mac CatalysttvOS 14.0+visionOS

``` source
static func reorder(
    displayed: UICellAccessory.DisplayedState = .whenEditing,
    options: UICellAccessory.ReorderOptions = ReorderOptions()
) -> UICellAccessory
```

## Parameters 

`displayed`  

The cell-editing states that the reorder accessory appears in. This parameter has a default value of UICellAccessory.DisplayedState.whenEditing.

`options`  

Configuration options for the reorder accessory. See UICellAccessory.ReorderOptions for possible configuration options.

## Return Value

A configured reorder cell accessory. This accessory is three horizontal lines with the default system gray color. This accessory appears on the trailing edge of the cell.

## Discussion

If your collection view supports interactive reordering of its cells, a user can drag the cell by its reorder accessory to change the order of the cell in the collection view.

## See Also

### Creating a reorder accessory

struct ReorderOptions

Configuration options for a reorder accessory.

