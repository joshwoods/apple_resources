

- CallKit
-  CXError 

Structure

# CXError

Error codes for the CallKit errors.

iOS 10.0+iPadOS 10.0+Mac Catalyst 10.0+visionOS 1.0+watchOS 9.0+

``` source
struct CXError
```

## Topics

### Constants

static var invalidArgument: CXError.Code

The argument is invalid.

static var unentitled: CXError.Code

The caller doesn’t have the correct entitlement.

static var unknownError: CXError.Code

An unknown error occurred.

### Type Properties

static var missingVoIPBackgroundMode: CXError.Code

static var errorDomain: String

### Enumerations

enum Code

Error codes for the CallKit errors.

## Relationships

### Conforms To

- CustomNSError
- Equatable
- Error
- Hashable
- Sendable

## See Also

### Handling Errors

enum CXCallEndedReason

The reason that a call ended.

enum Code

Error codes for the CallKit errors.

struct CXErrorCodeIncomingCallError

Codes for errors that occur during incoming calls.

enum Code

Codes for errors that occur during incoming calls.

struct CXErrorCodeNotificationServiceExtensionError

Errors that can occur when reporting new, incoming VoIP calls.

let CXErrorDomain: String

The domain for CallKit errors.

let CXErrorDomainIncomingCall: String

The domain for errors that occur during incoming calls.

