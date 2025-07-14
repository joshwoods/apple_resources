

- RealityKit
-  Reverb 

Structure

# Reverb

The reverberation RealityKit applies to spatial audio sources.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
struct Reverb
```

## Overview

You can configure the reverb for spatial audio sources in your RealityKit content with the ReverbComponent.

```
let cinema = Entity()
let reverb: Reverb = .preset(.mediumRoomDry)
cinema.components.set(ReverbComponent(reverb: reverb)
```

## Topics

### Structures

struct Preset

Reverbs defined by a preset environment.

### Operators

static func == (Reverb, Reverb) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Instance Properties

var hashValue: Int

The hash value.

### Instance Methods

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

### Type Properties

static let anechoic: Reverb

A reverb instance that applies no reverberation to spatial audio sources.

### Type Methods

static func preset(Reverb.Preset) -> Reverb

Returns a reverb instance that you can set on a reverb component.

### Default Implementations

Equatable Implementations

## Relationships

### Conforms To

- Equatable
- Hashable
- Sendable

## See Also

### Reverb

struct Preset

Reverbs defined by a preset environment.

struct ReverbComponent

A component that defines the reverberation of spatial audio sources.

