

- RealityKit
- SimpleMaterial
-  color 

Instance Property

# color

The material’s color.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS

``` source
var color: SimpleMaterial.BaseColor { get set }
```

## See Also

### Characterizing a material

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

var roughness: MaterialScalarParameter

The roughness of the material.

typealias Parameters

The parameter type that custom materials uses for properties the framework passes to shader functions.

