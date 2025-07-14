

- App Intents
- IntentFile
-  IntentFile.IntentFileError 

Enumeration

# IntentFile.IntentFileError

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
enum IntentFileError
```

## Topics

### Operators

static func == (IntentFile.IntentFileError, IntentFile.IntentFileError) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Enumeration Cases

case failedToLoadData

case failedToLoadFile

### Instance Properties

var errorCode: Int

The error code within the given domain.

var errorUserInfo: [String : Any]

The user-info dictionary.

var hashValue: Int

The hash value.

### Instance Methods

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

### Type Properties

static var errorDomain: String

The domain of the error.

### Default Implementations

CustomNSError Implementations

Equatable Implementations

Error Implementations

## Relationships

### Conforms To

- Copyable
- CustomNSError
- Equatable
- Error
- Hashable
- Sendable

