

- RealityKit
- ObjectCaptureSession
- ObjectCaptureSession.Tracking
-  ObjectCaptureSession.Tracking.Reason 

Enumeration

# ObjectCaptureSession.Tracking.Reason

The reason that tracking quality has degraded.

RealityKitSwiftUIiOS 17.0+iPadOS 17.0+

``` source
enum Reason
```

## Topics

### Operators

static func == (ObjectCaptureSession.Tracking.Reason, ObjectCaptureSession.Tracking.Reason) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Enumeration Cases

case excessiveMotion

The device is moving too fast for accurate tracking.

case initializing

Tracking is still initializing, usually at the start of a new session.

case insufficientFeatures

The scene does not contain enough distinguishable features for accurate camera tracking.

case relocalizing

The session is attempting to resume tracking after an interruption, such as the app being paused.

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

