

- DockKit
- DockAccessory
-  DockAccessory.TrackedObject 

Structure

# DockAccessory.TrackedObject

The state of a tracked object in the active tracking session.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+

``` source
struct TrackedObject
```

## Topics

### Operators

static func == (DockAccessory.TrackedObject, DockAccessory.TrackedObject) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Instance Properties

var identifier: UUID

A unique identifier for the tracked object. This identifier persists as long as the dock tracks the object. The value is random and doesn’t persist across sessions.

var rect: CGRect

The bounding box rectangle of the tracked object in the frame.

var saliencyRank: Int?

The saliency rank of the object the dock is tracking. A lower rank indicates higher importance of the object. This property is `nil` if the saliency ranking isn’t set or the object isn’t salient.

### Default Implementations

Equatable Implementations

## Relationships

### Conforms To

- Equatable
- Sendable

