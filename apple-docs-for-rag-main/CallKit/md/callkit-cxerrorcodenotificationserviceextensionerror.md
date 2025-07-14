

- CallKit
-  CXErrorCodeNotificationServiceExtensionError 

Structure

# CXErrorCodeNotificationServiceExtensionError

Errors that can occur when reporting new, incoming VoIP calls.

iOS 14.5+iPadOS 14.5+Mac Catalyst 14.5+visionOS 1.0+watchOS 9.0+

``` source
struct CXErrorCodeNotificationServiceExtensionError
```

## Overview

The system can return these errors to the reportNewIncomingVoIPPushPayload(_:completion:) method’s completion handler.

## Topics

### Understanding Error Codes

static var invalidClientProcess: CXErrorCodeNotificationServiceExtensionError.Code

An error indicating that an invalid client process reported the incoming call.

static var missingNotificationFilteringEntitlement: CXErrorCodeNotificationServiceExtensionError.Code

An error indicating that the notification service extension is missing the required filtering entitlement.

static var unknown: CXErrorCodeNotificationServiceExtensionError.Code

An error that occurs when there is an unknown problem.

enum Code

Constants for errors returned when reporting new, incoming VoIP calls.

### Type Properties

static var errorDomain: String

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

struct CXErrorCodeIncomingCallError

Codes for errors that occur during incoming calls.

enum Code

Codes for errors that occur during incoming calls.

let CXErrorDomain: String

The domain for CallKit errors.

let CXErrorDomainIncomingCall: String

The domain for errors that occur during incoming calls.

