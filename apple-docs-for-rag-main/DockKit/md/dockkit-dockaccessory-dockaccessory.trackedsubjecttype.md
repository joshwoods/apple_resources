

- DockKit
- DockAccessory
-  DockAccessory.TrackedSubjectType 

Enumeration

# DockAccessory.TrackedSubjectType

The subjects that the dock can track.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+

``` source
enum TrackedSubjectType
```

## Topics

### Operators

static func == (DockAccessory.TrackedSubjectType, DockAccessory.TrackedSubjectType) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Enumeration Cases

case object(DockAccessory.TrackedObject)

Tracked subject contains an object.

case person(DockAccessory.TrackedPerson)

Tracked subject contains a person.

### Default Implementations

Equatable Implementations

## Relationships

### Conforms To

- Equatable
- Sendable

