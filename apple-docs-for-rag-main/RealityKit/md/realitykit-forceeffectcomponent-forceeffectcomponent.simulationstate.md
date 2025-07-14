

- RealityKit
- ForceEffectComponent
-  ForceEffectComponent.SimulationState 

Enumeration

# ForceEffectComponent.SimulationState

The simulation runtime states.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
enum SimulationState
```

## Topics

### Operators

static func == (ForceEffectComponent.SimulationState, ForceEffectComponent.SimulationState) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Enumeration Cases

case pause

The simulation will pause.

case resume

The simulation will resume, if paused.

case start

The simulation will start, and its time set to zero. The simulation will restart if already started.

### Instance Properties

var hashValue: Int

The hash value.

### Instance Methods

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

### Default Implementations

Equatable Implementations

## Relationships

### Conforms To

- Copyable
- Equatable
- Hashable

