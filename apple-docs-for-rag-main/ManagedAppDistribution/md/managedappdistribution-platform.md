

- ManagedAppDistribution
-  Platform 

Structure

# Platform

The supported platform for the app.

iOS 17.2+iPadOS 17.2+visionOS 2.4+

``` source
struct Platform
```

## Topics

### Obtaining supported platforms

static var iOS: Platform

iOS is a supported platform.

static var macOS: Platform

macOS is a supported platform.

### Inspecting the object

var description: String

A textual representation of this instance.

### Operators

static func == (Platform, Platform) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Instance Properties

var hashValue: Int

The hash value.

### Instance Methods

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

### Type Properties

static var visionOS: Platform

visionOS is a supported platform.

### Default Implementations

Equatable Implementations

## Relationships

### Conforms To

- CustomStringConvertible
- Equatable
- Hashable
- Sendable

