

- Foundation
- NSUserActivity
-  NSUserActivity.TypedPayloadError 

Enumeration

# NSUserActivity.TypedPayloadError

An enumeration that describes the error types for getting and setting a typed payload.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
enum TypedPayloadError
```

## Overview

Use this enumeration to manage errors from typedPayload(_:) and setTypedPayload(_:).

## Topics

### Typed payload errors

case encodingError

An encoding error that indicates that the content failed to encode into a valid dictionary.

case invalidContent

A decoding error that indicates that the user info dictionary is empty or invalid.

## Relationships

### Conforms To

- Copyable
- Equatable
- Error
- Hashable
- Sendable

## See Also

### Managing type-safe access to user info

func setTypedPayload&lt;T>(T) throws

Encodes the specified payload into the user activity’s user info dictionary.

func typedPayload&lt;T>(T.Type) throws -> T

Decodes the user activity’s user info dictionary as an instance of the specified type.

