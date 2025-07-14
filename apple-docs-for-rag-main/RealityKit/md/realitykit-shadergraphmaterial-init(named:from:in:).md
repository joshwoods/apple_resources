

- RealityKit
- ShaderGraphMaterial
-  init(named:from:in:) 

Initializer

# init(named:from:in:)

Loads a ShaderGraphMaterial from a bundle.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 1.0+

``` source
init(
    named name: String,
    from file: String,
    in bundle: Bundle? = nil
) async throws
```

## Parameters 

`name`  

The name of the ShaderGraphMaterial within the file. For USD files, this is the full path of the material prim (such as “/Root/MyMaterial”).

`file`  

The name of the file within the bundle.

`bundle`  

The bundle containing the resource. Specify nil to search the app’s main bundle.

## Return Value

A ShaderGraphMaterial object from the file with the name specified.

## Discussion

Supported file formats are USD (.usd, .usda, .usdc, .usdz) and Reality File (.reality).

