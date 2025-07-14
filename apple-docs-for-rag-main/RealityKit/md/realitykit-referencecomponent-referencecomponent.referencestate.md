

- RealityKit
- ReferenceComponent
-  ReferenceComponent.ReferenceState 

Enumeration

# ReferenceComponent.ReferenceState

Defines the current loading state of the referenced entity.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
enum ReferenceState
```

## Topics

### Operators

static func == (ReferenceComponent.ReferenceState, ReferenceComponent.ReferenceState) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Enumeration Cases

case loaded

The reference is loaded.

case loading

The reference is loading.

case notLoaded

The reference isn’t loaded.

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

