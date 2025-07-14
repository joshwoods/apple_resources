

- UIKit
- UICellAccessory
-  label(text:displayed:options:) 

Type Method

# label(text:displayed:options:)

Creates a label system accessory with the specified text, display state, and configuration options.

iOS 14.0+iPadOS 14.0+Mac CatalysttvOS 14.0+visionOS

``` source
static func label(
    text: String,
    displayed: UICellAccessory.DisplayedState = .always,
    options: UICellAccessory.LabelOptions = LabelOptions()
) -> UICellAccessory
```

## Parameters 

`text`  

The text for the label to display.

`displayed`  

The cell-editing states that the label accessory appears in. This parameter has a default value of UICellAccessory.DisplayedState.always.

`options`  

Configuration options for the label. See UICellAccessory.LabelOptions for possible configuration options.

## Return Value

A configured label cell accessory. This accessory appears on the trailing edge of the cell.

## Discussion

Use this cell accessory to display a short string of text, like a small number showing the count for the associated item.

## See Also

### Creating a label accessory

struct LabelOptions

Configuration options for a label accessory.

