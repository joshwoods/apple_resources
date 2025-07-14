

- ProximityReader
- ProximityReaderDiscovery
-  ProximityReaderDiscovery.ContentError 

Enumeration

# ProximityReaderDiscovery.ContentError

Errors that indicate a problem occurred when getting or showing content.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+visionOS 2.0+

``` source
enum ContentError
```

## Topics

### Getting the errors

case contentNotFound

An error that indicates the requested content isn’t available.

case contentDisplayFailed

An error that indicates an issue occurred when trying to display the requested content.

case notSupported

An error that indicates the current device doesn’t support the requested content.

case networkUnavailable

An error that indicates the system can’t reach the network.

case systemBusy

An error that indicates the system is busy.

case unknown

An error that indicates the framework encountered a problem that the system can’t interpret.

### Operators

static func == (ProximityReaderDiscovery.ContentError, ProximityReaderDiscovery.ContentError) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Instance Properties

var hashValue: Int

The hash value.

### Instance Methods

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

### Default Implementations

Equatable Implementations

Error Implementations

LocalizedError Implementations

## Relationships

### Conforms To

- Copyable
- Equatable
- Error
- Hashable
- LocalizedError
- Sendable

