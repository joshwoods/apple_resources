

- Model I/O
- MDLMaterial
-  init(name:scatteringFunction:) 

Initializer

# init(name:scatteringFunction:)

Initializes a material

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
init(
    name: String,
    scatteringFunction: MDLScatteringFunction
)
```

## Parameters 

`name`  

A descriptive name for the material.

`scatteringFunction`  

The collection of material properties that define the material’s response to light. For details, see the scatteringFunction property.

## Return Value

A new material object.

## Discussion

To use the newly created material with a 3D object, assign it to the the material property of a MDLSubmesh instance.

