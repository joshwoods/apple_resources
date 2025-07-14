

- MediaExtension
- MERAWProcessingParameter
- MERAWProcessingParameter.SubGroup
-  init(name:description:parameters:) 

Initializer

# init(name:description:parameters:)

Creates a sub group parameter object with the parameters value.

macOS 15.0+

``` source
init(
    name: String,
    description: String,
    parameters: [MERAWProcessingParameter]
)
```

## Parameters 

`name`  

A localized human-readable name for the parameter, suitable for displaying in application UI.

`description`  

A localized description of the parameter, suitable for displaying in a tool tip or similar explanatory UI.

`parameters`  

The array of MERAWProcessingParameter objects in the sub group.

## Return Value

An instance of MERAWProcessingParameter.SubGroup.

