

- Model I/O
- MDLMaterial
-  name 

Instance Property

# name

A descriptive name for the material.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
var name: String { get set }
```

## Discussion

This name isn’t used in rendering, but it can be useful for debugging and organizing the materials used in a project. When you load materials from an asset file with the MDLAsset class, Model I/O uses names assigned in the asset file where supported by the file format.

## See Also

### Using a material

var materialFace: MDLMaterialFace

The surface of an object.

