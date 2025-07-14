

- CallKit
-  CXCallEndedReason 

Enumeration

# CXCallEndedReason

The reason that a call ended.

iOS 10.0+iPadOS 10.0+Mac Catalyst 10.0+visionOS 1.0+watchOS 9.0+

``` source
enum CXCallEndedReason
```

## Overview

Pass these values to the reportCall(with:endedAt:reason:) method.

## Topics

### Constants

case failed

An error occurred while attempting to service the call.

case remoteEnded

The remote party explicitly ended the call.

case unanswered

The call never started connecting and was never explicitly ended, such as when an outgoing or incoming call times out.

case answeredElsewhere

Another device answered the call.

case declinedElsewhere

Another device declined the call.

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

struct CXError

Error codes for the CallKit errors.

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

