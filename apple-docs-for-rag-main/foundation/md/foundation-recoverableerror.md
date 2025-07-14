

- Foundation
-  RecoverableError 

Protocol

# RecoverableError

A specialized error that may be recoverable by presenting several potential recovery options to the user.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
protocol RecoverableError : Error
```

## Topics

### Instance Properties

var recoveryOptions: [String]

Provides a set of possible recovery options to present to the user.

**Required**

### Instance Methods

func attemptRecovery(optionIndex: Int) -> Bool

Attempt to recover from this error when the user selected the option at the given index. Returns true to indicate successful recovery, and false otherwise.

**Required**

func attemptRecovery(optionIndex: Int, resultHandler: (Bool) -> Void)

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

protocol LocalizedError

A specialized error that provides localized messages describing the error and why it occurred.

protocol CustomNSError

A specialized error that provides a domain, error code, and user-info dictionary.

