

- RealityKit
- SimpleMaterial
-  metallic 

Instance Property

# metallic

A value that you set to control whether the material has a metallic look.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+visionOS

``` source
var metallic: MaterialScalarParameter { get set }
```

## Discussion

This property defines whether a material is dielectric (`0.0`) or a metallic (`1.0`). Although this property can be set to any value between `0` and `1`, to create a realistic material, set it to either `0` or `1`.).

Dielectric materials  
These are materials that simulate real-world materials that are poor conductors. In these materials, light travels into the surface of the material and the color is mostly controlled by the color of the sub-surface. Typical examples of dielectric materaisl include organic materials, plastics, and industrial minerals such as sand, limestone, marble, clay and salt.

Metallic  
A metallic (or *conductive*) material reflects light differently than dielectric ones. The overall color is caused by an immediate re-emission of the light from the entity’s surface. Typical examples of metallic materials include aluminum, chassis metal, chromium, copper, gold, silver, and titanium

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

var roughness: MaterialScalarParameter

The roughness of the material.

typealias Parameters

The parameter type that custom materials uses for properties the framework passes to shader functions.

