

- UIKit
- UICellAccessory
-  disclosureIndicator(displayed:options:) 

Type Method

# disclosureIndicator(displayed:options:)

Creates a disclosure indicator system accessory with the specified display state and configuration options.

iOS 14.0+iPadOS 14.0+Mac CatalysttvOS 14.0+visionOS

``` source
static func disclosureIndicator(
    displayed: UICellAccessory.DisplayedState = .always,
    options: UICellAccessory.DisclosureIndicatorOptions = DisclosureIndicatorOptions()
) -> UICellAccessory
```

## Parameters 

`displayed`  

The cell-editing states that the disclosure indicator appears in. This parameter has a default value of UICellAccessory.DisplayedState.always.

`options`  

Configuration options for the disclosure indicator. See UICellAccessory.DisclosureIndicatorOptions for possible configuration options.

## Return Value

A configured disclosure indicator cell accessory. This accessory is a disclosure chevron that points in the trailing direction. This accessory appears on the trailing edge of the cell.

## Discussion

Use this cell accessory to indicate that users can tap on the cell to disclose additional content.

## See Also

### Creating a disclosure indicator

struct DisclosureIndicatorOptions

Configuration options for a disclosure indicator.

