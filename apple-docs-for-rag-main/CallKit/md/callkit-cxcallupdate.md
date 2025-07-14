

- CallKit
-  CXCallUpdate 

Class

# CXCallUpdate

An encapsulation of new and changed information about a call.

iOS 10.0+iPadOS 10.0+Mac Catalyst 10.0+visionOS 1.0+watchOS 9.0+

``` source
class CXCallUpdate
```

## Mentioned in 

Making and receiving VoIP calls

## Overview

CXCallUpdate objects are used by the system to communicate changes to calls over time. Not every property on a CXCallUpdate object must be set each time, as each object includes only new and changed information. For example, when a call is started, only some properties may be known and included in the first CXCallUpdate object sent to the system, such as localizedCallerName. Later in the same call, other properties may change; for example, a call may be upgraded from audio only to audio and video, which would be reflected by a new CXCallUpdate object with its hasVideo property set to true.

When an incoming call is received, you construct a CXCallUpdate object specifying a localizedCallerName and pass that to the reportNewIncomingCall(with:update:completion:) method to notify the telephony provider.

When an active call is updated, you construct a CXCallUpdate object specifying any updated information and pass that to the reportCall(with:updated:) method. For example, if a user changes their contact information during a call, you could notify the telephony provider of this change using a new CXCallUpdate object with the new value set to its remoteHandle property.

## Topics

### Accessing Call Update Attributes

var localizedCallerName: String?

The localized name of the caller.

var remoteHandle: CXHandle?

The handle for the remote party (for an incoming call, this is the caller; for an outgoing call, this is the callee).

var hasVideo: Bool

A Boolean value that indicates whether the call includes video in addition to audio.

var supportsGrouping: Bool

A Boolean value that indicates whether the call can be grouped with other calls.

var supportsUngrouping: Bool

A Boolean value that indicates whether the call can be ungrouped from other calls.

var supportsHolding: Bool

A Boolean value that indicates whether the call can be placed on hold or removed from hold.

var supportsDTMF: Bool

A Boolean value that indicates whether the call can send DTMF (dual tone multifrequency) tones via hard pause digits or in-call keypad entries.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCopying
- NSObjectProtocol

## See Also

### Incoming calls

Responding to VoIP Notifications from PushKit

Receive incoming Voice-over-IP (VoIP) push notifications and use them to display the system call interface to the user.

class CXAnswerCallAction

An encapsulation of the act of answering an incoming call.

