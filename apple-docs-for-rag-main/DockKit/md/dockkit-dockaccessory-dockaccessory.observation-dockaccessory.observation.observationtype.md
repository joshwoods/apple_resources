

- DockKit
- DockAccessory
- DockAccessory.Observation
-  DockAccessory.Observation.ObservationType 

Enumeration

# DockAccessory.Observation.ObservationType

The available observation types.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+

``` source
enum ObservationType
```

## Topics

### Operators

static func == (DockAccessory.Observation.ObservationType, DockAccessory.Observation.ObservationType) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Enumeration Cases

case humanBody

The frame contains a human body.

case humanFace

The frame contains a human face.

case object

The frame contains an object other than a human face or body.

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

- Equatable
- Hashable
- Sendable

