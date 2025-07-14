

- SwiftUI
- DisclosureTableRow
-  init(\_:isExpanded:content:) 

Initializer

# init(\_:isExpanded:content:)

Creates a disclosure group with the given value and table rows, and a binding to the expansion state (expanded or collapsed).

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+visionOS 1.0+

``` source
init(
    _ value: Value,
    isExpanded: Binding? = nil,
    @TableRowBuilder content: @escaping () -> Content
) where Label == TableRow, Value == Content.TableRowValue
```

## Parameters 

`value`  

The value of the disclosable table row.

`isExpanded`  

A binding to a Boolean value that determines the group’s expansion state (expanded or collapsed).

`content`  

The table row shown when the disclosure group expands.

