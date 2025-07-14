

- RealityKit
- ShaderGraphMaterial
-  init(materialXLabel:data:) 

Initializer

# init(materialXLabel:data:)

Loads a ShaderGraphMaterial from MaterialX data.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 1.0+

``` source
init(
    materialXLabel: String,
    data: Data
) async throws
```

## Parameters 

`materialXLabel`  

The name of the ShaderGraphMaterial in the MaterialX data.

`data`  

The data containing the MaterialX file contents.

## Return Value

A ShaderGraphMaterial object from the data with the label specified.

