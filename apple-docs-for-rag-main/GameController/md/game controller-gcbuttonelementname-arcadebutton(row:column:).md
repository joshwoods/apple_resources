

- Game Controller
- GCButtonElementName
-  arcadeButton(row:column:) 

Type Method

# arcadeButton(row:column:)

Returns the name of the arcade stick button at the specified location.

iOS 17.0+iPadOS 17.0+Mac CatalystmacOS 14.0+tvOS 17.0+visionOS

``` source
static func arcadeButton(
    row: Int,
    column: Int
) -> GCButtonElementName
```

## Parameters 

`row`  

The row on the arcade stick that the button appears in, where `0` is the bottom row.

`column`  

The column on the arcade stick that the button appears in, where `0` is the column nearest to the lever or direction buttons.

## Return Value

The name of an arcade stick button.

