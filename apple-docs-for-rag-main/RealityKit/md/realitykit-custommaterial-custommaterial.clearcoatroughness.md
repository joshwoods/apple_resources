

- RealityKit
- CustomMaterial
-  CustomMaterial.ClearcoatRoughness 

Structure

# CustomMaterial.ClearcoatRoughness

An object that defines the degree to which an entity’s clear, shiny coating scatters light to create soft highlights.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+

``` source
struct ClearcoatRoughness
```

## Overview

An entity in RealityKit can display a clearcoat, which is a separate layer of transparent specular highlights used to simulate a clear coating, like on a car or the surface of lacquered objects. Use this object to specify a clearcoat roughness value and indicate how much the clearcoat scatters light that bounces off of it, which softens and disperses the highlights.

For information, see clearcoatRoughness.

## Topics

### Creating a clearcoat roughness object

init(floatLiteral: Float)

Creates a clearcoat object using a single value.

init(scale: Float, texture: CustomMaterial.Texture?)

Creates a clearcoat object using a single value or a texture.

init(PhysicallyBasedMaterial.ClearcoatRoughness)

Creates a custom clearcoat object from a physically based material’s clearcoat property.

### Accessing clearcoat roughness values

var scale: Float

The clearcoat intensity specified as a single value.

var texture: CustomMaterial.Texture?

The clearcoat intensity specified using a UV-mapped image.

typealias FloatLiteralType

A type that represents a floating-point literal.

## Relationships

### Conforms To

- ExpressibleByFloatLiteral

