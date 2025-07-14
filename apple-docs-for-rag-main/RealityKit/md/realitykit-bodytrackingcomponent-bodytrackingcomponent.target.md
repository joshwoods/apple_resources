

- RealityKit
- BodyTrackingComponent
-  BodyTrackingComponent.Target 

Enumeration

# BodyTrackingComponent.Target

Body-tracking settings for selecting a person to track.

iOS 13.0+iPadOS 13.0+Mac Catalyst 14.0+

``` source
enum Target
```

## Topics

### Body tracking target types

case any

Any person that is detected in front of the camera.

case body(identifier: UUID)

A person detected by ARKit.

### Comparing targets

static func == (BodyTrackingComponent.Target, BodyTrackingComponent.Target) -> Bool

Indicates whether two targets are equal.

static func != (Self, Self) -> Bool

Returns a Boolean value indicating whether two values are not equal.

func hash(into: inout Hasher)

Hashes the essential components of the target by feeding them into the given hash function.

var hashValue: Int

The hash value.

### Default Implementations

Equatable Implementations

## Relationships

### Conforms To

- Equatable
- Hashable

## See Also

### Selecting a body to track

var target: BodyTrackingComponent.Target

The body-tracking setting.

