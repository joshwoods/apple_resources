

- RealityKit
- ShaderGraphMaterial
-  init(named:from:) 

Initializer

# init(named:from:)

Loads a ShaderGraphMaterial from a named material within a USD file.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 1.0+

``` source
init(
    named name: String,
    from data: Data
) async throws
```

## Parameters 

`name`  

The name of the ShaderGraphMaterial within the USD file.

`data`  

A data object containing USD file data

## Return Value

A ShaderGraphMaterial object from the file with the name specified.

## Discussion

Supported file formats are USD (.usd, .usda, .usdc, .usdz)

