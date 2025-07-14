

- RealityKit
-  UnsafeForceEffectBuffer 

Structure

# UnsafeForceEffectBuffer

Provides access to physics body parameters from the effect’s update function or event handler.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
struct UnsafeForceEffectBuffer
```

## Overview

This struct is a transient buffer view of underlying data, and is only available in effect’s update function or update closure.

## Topics

### Structures

struct Iterator

Iterates over all elements of the `UnsafeForceEffectBuffer`.

### Instance Properties

var count: Int

Returns the number of elements in the buffer.

### Instance Methods

func makeIterator() -> UnsafeForceEffectBuffer&lt;T>.Iterator

Returns an iterator for the sequence.

### Subscripts

subscript(Int) -> T

Returns an element by index.

### Type Aliases

typealias Element

A type representing the sequence’s elements.

### Default Implementations

Sequence Implementations

## Relationships

### Conforms To

- Sequence

## See Also

### Updating effects

func update(parameters: inout ForceEffectParameters)

Defines how the custom force effect computes forces at each physics simulation step.

**Required** Default implementation provided.

static func register(((inout ForceEffectEvent&lt;Self>) -> Void)?)

Registers the custom effect.

struct PhysicsBodyParameterTypes

Defines which rigid body inputs are required by a force effect’s update handler.

struct ForceEffectParameters

The force effect input data to the effect’s update handler or closure.

struct ForceEffectEvent

A struct that defines the arguments to the custom force effect update closure.

