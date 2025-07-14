

- RealityKit
- ReferenceComponent
-  ReferenceComponent.LoadingPolicy 

Enumeration

# ReferenceComponent.LoadingPolicy

Describes when a referenced entity loads.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
enum LoadingPolicy
```

## Topics

### Operators

static func == (ReferenceComponent.LoadingPolicy, ReferenceComponent.LoadingPolicy) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Enumeration Cases

case immediate

Loads the contents from the referenced entity file immediately when the root entity loads.

case onDemand

Loads the contents from the referenced entity file when your app tells it to.

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

