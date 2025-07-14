

- CallKit
-  CXAnswerCallAction 

Class

# CXAnswerCallAction

An encapsulation of the act of answering an incoming call.

iOS 10.0+iPadOS 10.0+Mac Catalyst 10.0+visionOS 1.0+watchOS 9.0+

``` source
class CXAnswerCallAction
```

## Overview

CXAnswerCallAction is a concrete subclass of CXCallAction.

When an incoming call is allowed by the system and approved by the user, the provider sends provider(_:perform:) to its delegate. The provider’s delegate calls the fulfill() method to indicate that the action was successfully performed. To indicate that the call connected at a time other than the current time, you can instead call the fulfill(withDateConnected:).

## Topics

### Completing Actions

func fulfill(withDateConnected: Date)

Reports the successful execution of the action at the specified time.

## Relationships

### Inherits From

- CXCallAction

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSCopying
- NSObjectProtocol
- NSSecureCoding

## See Also

### Incoming calls

Responding to VoIP Notifications from PushKit

Receive incoming Voice-over-IP (VoIP) push notifications and use them to display the system call interface to the user.

class CXCallUpdate

An encapsulation of new and changed information about a call.

