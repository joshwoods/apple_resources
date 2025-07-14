

- RealityKit
- PhysicallyBasedMaterial
-  PhysicallyBasedMaterial.Program 

Class

# PhysicallyBasedMaterial.Program

An object that represents the backing shader compilation required for physically based materials.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
final class Program
```

## Overview

You can use this type to control when RealityKit compiles shaders, and to initialize `PhysicallyBasedMaterial` objects with more predicitable loading performance.

When initializing a `PhysicallyBasedMaterial` this way, a `Program` object is created first asynchronously, which is used to cache the material’s shader program so the `PhysicallyBasedMaterial` can be loaded immediately later.

For example:

```
// Initialize descriptor with desired properties
var descriptor = PhysicallyBasedMaterial.Descriptor()
descriptor.blendMode = .add

// Create program object
let program = await PhysicallyBasedMaterial.Program(descriptor: descriptor)

// Create material (returns immediately)
let material = PhysicallyBasedMaterial(program: program)
```

## Topics

### Structures

struct Descriptor

Specifies all parameters necessary to initialize `PhysicallyBasedMaterial` programs

### Operators

static func == (PhysicallyBasedMaterial.Program, PhysicallyBasedMaterial.Program) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Initializers

init(descriptor: PhysicallyBasedMaterial.Program.Descriptor) async

### Instance Properties

let descriptor: PhysicallyBasedMaterial.Program.Descriptor

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

