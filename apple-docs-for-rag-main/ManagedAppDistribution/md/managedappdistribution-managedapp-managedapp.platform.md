

- ManagedAppDistribution
- ManagedApp
-  ManagedApp.Platform 

Structure

# ManagedApp.Platform

The supported platform for the app.

iOS 17.2+iPadOS 17.2+visionOS 2.4+

``` source
struct Platform
```

## Topics

### Operators

static func == (ManagedApp.Platform, ManagedApp.Platform) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Instance Properties

var description: String

A textual representation of this instance.

var hashValue: Int

The hash value.

### Instance Methods

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

### Type Properties

static var iOS: ManagedApp.Platform

iOS is a supported platform.

static var macOS: ManagedApp.Platform

macOS is a supported platform.

static var visionOS: ManagedApp.Platform

visionOS is a supported platform.

### Default Implementations

Equatable Implementations

## Relationships

### Conforms To

- CustomStringConvertible
- Equatable
- Hashable
- Sendable

## See Also

### Obtaining platform and requirement information

let platform: Platform

The platform of the app.

let requirements: String?

The app’s localized operating system compatibility requirements.

