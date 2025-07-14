

- RealityKit
- ShaderGraphMaterial
-  init(named:from:) 

Initializer

# init(named:from:)

Loads a ShaderGraphMaterial from a url.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 1.0+

``` source
init(
    named name: String,
    from url: URL
) async throws
```

## Parameters 

`name`  

The name of the ShaderGraphMaterial within the file. For USD files, this is the full path of the material prim (such as “/Root/MyMaterial”).

`url`  

The path or address of the file containing the ShaderGraphMaterial.

## Return Value

A ShaderGraphMaterial object from the file with the name specified.

## Discussion

Supported file formats are USD (.usd, .usda, .usdc, .usdz) and Reality File (.reality).

