

- MediaExtension
- MERAWProcessingParameter
- MERAWProcessingParameter.ListElement
-  init(name:description:elementID:) 

Initializer

# init(name:description:elementID:)

Creates a list element parameter object with the element id value.

macOS 15.0+

``` source
init(
    name: String,
    description: String,
    elementID: Int
)
```

## Parameters 

`name`  

A localized human-readable name for the parameter, suitable for displaying in application UI.

`description`  

A localized description of the parameter, suitable for displaying in a tool tip or similar explanatory UI.

`elementID`  

A unique number in the list which represents this list option.

## Return Value

An instance of MERAWProcessingParameter.ListElement.

