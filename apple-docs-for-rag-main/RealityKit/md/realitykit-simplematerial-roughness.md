

- RealityKit
- SimpleMaterial
-  roughness 

Instance Property

# roughness

The roughness of the material.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+visionOS

``` source
var roughness: MaterialScalarParameter { get set }
```

## See Also

### Characterizing a material

var color: SimpleMaterial.BaseColor

The material’s color.

var baseColor: MaterialColorParameter

The base color of the material.

Deprecated

typealias BaseColor

The type used to represent base color.

var tintColor: UIColor

A tint color applied to the base color in macOS.

Deprecated

var tintColor: NSColor

A tint color applied to the base color in macOS.

Deprecated

typealias Texture

The type used to represent textures.

var metallic: MaterialScalarParameter

A value that you set to control whether the material has a metallic look.

typealias Parameters

The parameter type that custom materials uses for properties the framework passes to shader functions.

