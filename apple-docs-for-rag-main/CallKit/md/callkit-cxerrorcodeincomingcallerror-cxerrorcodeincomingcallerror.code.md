

- CallKit
- CXErrorCodeIncomingCallError
-  CXErrorCodeIncomingCallError.Code 

Enumeration

# CXErrorCodeIncomingCallError.Code

Codes for errors that occur during incoming calls.

iOS 10.0+iPadOS 10.0+Mac Catalyst 10.0+visionOS 1.0+watchOS 9.0+

``` source
enum Code
```

## Topics

### Errors

case unknown

An unknown error occurred.

case unentitled

The app isn’t entitled to receive incoming calls.

case callUUIDAlreadyExists

The incoming call UUID already exists.

case filteredByDoNotDisturb

The incoming call is filtered because Do Not Disturb is active and the incoming caller is not a VIP.

case filteredByBlockList

The incoming call is filtered because the incoming caller has been blocked by the user.

### Enumeration Cases

case filteredDuringRestrictedSharingMode

case callIsProtected

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

enum Code

Error codes for the CallKit errors.

struct CXErrorCodeIncomingCallError

Codes for errors that occur during incoming calls.

struct CXErrorCodeNotificationServiceExtensionError

Errors that can occur when reporting new, incoming VoIP calls.

let CXErrorDomain: String

The domain for CallKit errors.

let CXErrorDomainIncomingCall: String

The domain for errors that occur during incoming calls.

