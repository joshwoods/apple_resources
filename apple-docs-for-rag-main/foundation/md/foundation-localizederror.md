

- Foundation
-  LocalizedError 

Protocol

# LocalizedError

A specialized error that provides localized messages describing the error and why it occurred.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
protocol LocalizedError : Error
```

## Topics

### Instance Properties

var errorDescription: String?

**Required** Default implementation provided.

var failureReason: String?

**Required** Default implementation provided.

var helpAnchor: String?

**Required** Default implementation provided.

var recoverySuggestion: String?

**Required** Default implementation provided.

## Relationships

### Inherits From

- Error
- Sendable

## See Also

### User-Relevant Errors

protocol Error : Sendable

A type representing an error value that can be thrown.

class NSError

Information about an error condition including a domain, a domain-specific error code, and application-specific information.

protocol RecoverableError

A specialized error that may be recoverable by presenting several potential recovery options to the user.

protocol CustomNSError

A specialized error that provides a domain, error code, and user-info dictionary.

