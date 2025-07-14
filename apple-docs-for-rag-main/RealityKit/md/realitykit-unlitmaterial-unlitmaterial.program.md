

- RealityKit
- UnlitMaterial
-  UnlitMaterial.Program 

Class

# UnlitMaterial.Program

An object that represents the backing shader compilation required for unlit materials.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
final class Program
```

## Overview

You can use this type to control when RealityKit compiles shaders, and to initialize `UnlitMaterial` objects with more predicitable loading performance.

When initializing an `UnlitMaterial` this way, a `Program` object is created first asynchronously, which is used to cache the material’s shader program so the `UnlitMaterial` can be loaded immediately later.

For example:

```
// Initialize descriptor with desired properties
var descriptor = UnlitMaterial.Descriptor()
descriptor.applyPostProcessToneMap = false

// Create program object
let program = await UnlitMaterial.Program(descriptor: descriptor)

// Create material (returns immediately)
let material = UnlitMaterial(program: program)
```

## Topics

### Structures

struct Descriptor

An object that specifies all parameters necessary to initialize `UnlitMaterial` programs

### Operators

static func == (UnlitMaterial.Program, UnlitMaterial.Program) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Initializers

init(descriptor: UnlitMaterial.Program.Descriptor) async

### Instance Properties

let descriptor: UnlitMaterial.Program.Descriptor

var hashValue: Int

The hash value.

### Instance Methods

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

### Default Implementations

Equatable Implementations

## Relationships

### Conforms To

- Equatable
- Hashable
- Sendable

