

- CallKit
-  CXErrorCodeIncomingCallError 

Structure

# CXErrorCodeIncomingCallError

Codes for errors that occur during incoming calls.

iOS 10.0+iPadOS 10.0+Mac Catalyst 10.0+visionOS 1.0+watchOS 9.0+

``` source
struct CXErrorCodeIncomingCallError
```

## Topics

### Errors

static var callUUIDAlreadyExists: CXErrorCodeIncomingCallError.Code

The incoming call UUID already exists.

static var filteredByBlockList: CXErrorCodeIncomingCallError.Code

The system is filtering the incoming call because the user is blocking it.

static var filteredByDoNotDisturb: CXErrorCodeIncomingCallError.Code

The system is filtering the incoming call because Do Not Disturb is active and the incoming caller isn’t a VIP.

static var unentitled: CXErrorCodeIncomingCallError.Code

The app doesn’t have the entitlement to receive incoming calls.

static var unknown: CXErrorCodeIncomingCallError.Code

An unknown error occurred.

### Type Properties

static var filteredDuringRestrictedSharingMode: CXErrorCodeIncomingCallError.Code

static var callIsProtected: CXErrorCodeIncomingCallError.Code

static var errorDomain: String

### Enumerations

enum Code

Codes for errors that occur during incoming calls.

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

struct CXError

Error codes for the CallKit errors.

enum Code

Error codes for the CallKit errors.

enum Code

Codes for errors that occur during incoming calls.

struct CXErrorCodeNotificationServiceExtensionError

Errors that can occur when reporting new, incoming VoIP calls.

let CXErrorDomain: String

The domain for CallKit errors.

let CXErrorDomainIncomingCall: String

The domain for errors that occur during incoming calls.

