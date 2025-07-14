

- UIKit
- UICellAccessory
-  outlineDisclosure(displayed:options:actionHandler:) 

Type Method

# outlineDisclosure(displayed:options:actionHandler:)

Creates an outline disclosure system accessory with the specified display state, configuration options, and optional action handler.

iOS 14.0+iPadOS 14.0+Mac CatalysttvOS 14.0+visionOS

``` source
static func outlineDisclosure(
    displayed: UICellAccessory.DisplayedState = .always,
    options: UICellAccessory.OutlineDisclosureOptions = OutlineDisclosureOptions(),
    actionHandler: UICellAccessory.ActionHandler? = nil
) -> UICellAccessory
```

## Parameters 

`displayed`  

The cell-editing states that the outline disclosure appears in. This parameter has a default value of UICellAccessory.DisplayedState.always.

`options`  

Configuration options for the outline disclosure. See UICellAccessory.OutlineDisclosureOptions for possible configuration options.

`actionHandler`  

An optional closure that the system calls when a user interacts with the outline disclosure.

## Return Value

A configured outline disclosure cell accessory. This accessory is a rotating chevron for use in outlines. In iOS and for headers in Mac Catalyst, this accessory appears on the trailing edge. For cells in Mac Catalyst, this accessory appears on the leading edge.

## Discussion

Use this cell accessory to indicate that an item can expand and collapse, and to enable the user to toggle between the expanded and collapsed states.

## See Also

### Creating an outline disclosure

struct OutlineDisclosureOptions

Configuration options for an outline disclosure.

