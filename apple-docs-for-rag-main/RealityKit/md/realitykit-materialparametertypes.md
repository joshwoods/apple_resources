

- RealityKit
-  MaterialParameterTypes 

Structure

# MaterialParameterTypes

A set of types that material parameters can use.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS

``` source
struct MaterialParameterTypes
```

## Overview

This class contains many nested types used to specify various properties of material.

Many material properties support more than one type of data. For example, you can specify baseColor using either a single `Float`, or a UV mapped image texture. MaterialParameterTypes and its nested symbols implement the ability to accept different data types for the same property.

## Topics

### Structures

struct TextureCoordinateTransform

An object that defines a transformation the framework applies to a material’s UV-mapped textures.

### Enumerations

enum BlendMode

Modes that describe how materials should be blended with content behind them.

enum FaceCulling

An object that defines how the system removes polygons before rendering a scene.

enum TriangleFillMode

An object that defines how the system rasterizes triangles and triangle strips

## See Also

### Material types

protocol Material

A type that describes the material aspects of a mesh, like color and texture.

typealias Color

An alias for the color type that’s appropriate for the current platform.

typealias Parameters

The parameter type that custom materials uses for properties the framework passes to shader functions.

struct MaterialParameters

enum MaterialColorParameter

The color parameter applied to a material.

enum MaterialScalarParameter

The scalar parameter applied to a material.

