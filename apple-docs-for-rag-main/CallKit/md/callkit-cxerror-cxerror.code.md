

- CallKit
- CXError
-  CXError.Code 

Enumeration

# CXError.Code

Error codes for the CallKit errors.

iOS 10.0+iPadOS 10.0+Mac Catalyst 10.0+visionOS 1.0+watchOS 9.0+

``` source
enum Code
```

## Topics

### Constants

case invalidArgument

The argument is invalid.

case unentitled

The caller doesn’t have the correct entitlement.

case unknownError

An unknown error occurred.

### Enumeration Cases

case missingVoIPBackgroundMode

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Handling Errors

enum CXCallEndedReason

The reason that a call ended.

struct CXError

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

