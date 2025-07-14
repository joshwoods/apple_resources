

- RealityKit
-  MaterialFunction 

Protocol

# MaterialFunction

The abstract superclass for objects representing compute functions for RealityKit custom materials .

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS

``` source
protocol MaterialFunction
```

## Overview

This class is the parent of, and contains common properties and methods for CustomMaterial.GeometryModifier and CustomMaterial.SurfaceShader. Don’t create an instance of this superclass yourself.

## Topics

### Instance Properties

var constantValues: MTLFunctionConstantValues

The constant values to use when RealityKit creates your function. These correspond to constants defined in your metal code.

**Required**

var library: any MTLLibrary

Metal Library containing the given function.

**Required**

var name: String

Name of function found in library

**Required**

## Relationships

### Conforming Types

- CustomMaterial.GeometryModifier
- CustomMaterial.SurfaceShader

## See Also

### Shaders

struct ShaderGraphMaterial

typealias FaceCulling

An alias for the cull mode object that’s appropriate for this material class.

typealias TriangleFillMode

An alias for the triangle fill mode object that’s appropriate for this material class.

Modifying RealityKit rendering using custom materials

Write Metal shader functions to implement custom rendering effects.

struct CustomMaterial

A material that works with custom Metal shader functions.

struct SurfaceShader

The custom material’s surface shader function.

struct GeometryModifier

The custom material’s optional shader function that can manipulate an entity’s vertex data.

class Program

An object that represents the backing shader compilation required for custom materials.

struct Descriptor

An object that specifies all parameters necessary to initialize `CustomMaterial` programs

enum CustomShaderStage

