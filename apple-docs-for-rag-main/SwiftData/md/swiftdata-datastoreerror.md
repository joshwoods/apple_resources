

- SwiftData
-  DataStoreError 

Enumeration

# DataStoreError

A type that describes a data store error.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 10.0+Swift 5.9+

``` source
enum DataStoreError
```

## Topics

### Getting error codes

case invalidPredicate

case preferInMemoryFilter

case preferInMemorySort

case unsupportedFeature

### Comparing errors

static func == (DataStoreError, DataStoreError) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Hashing errors

var hashValue: Int

The hash value.

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

### Default Implementations

Equatable Implementations

Error Implementations

## Relationships

### Conforms To

- Copyable
- Equatable
- Error
- Hashable
- Sendable

## See Also

### Errors

struct SwiftDataError

A type that describes a SwiftData error.

