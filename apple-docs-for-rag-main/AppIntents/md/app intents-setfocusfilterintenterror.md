

- App Intents
-  SetFocusFilterIntentError 

Enumeration

# SetFocusFilterIntentError

Errors that can occur when you try to retrieve the current Focus configuration settings.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
enum SetFocusFilterIntentError
```

## Topics

### Getting the error codes

case notFound

### Operators

static func == (SetFocusFilterIntentError, SetFocusFilterIntentError) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Enumeration Cases

case missingParameterValue

An error indicating that the intent has an invalid parameter value.

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

