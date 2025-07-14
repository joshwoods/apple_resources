

- CallKit
-  CXSetMutedCallAction 

Class

# CXSetMutedCallAction

An encapsulation of the act of muting or unmuting a call.

iOS 10.0+iPadOS 10.0+Mac Catalyst 10.0+visionOS 1.0+watchOS 9.0+

``` source
class CXSetMutedCallAction
```

## Overview

CXSetMutedCallAction is a concrete subclass of CXCallAction. When the user or the system mutes a call, the provider sends provider(_:perform:) to its delegate. The provider’s delegate calls the fulfill() method to indicate that the action was successfully performed. When a caller mutes a call, that caller is unable to communicate with other callers until they unmute the call. A muted caller still receives communication from other unmuted callers.

## Topics

### Creating New Actions

convenience init(call: UUID, muted: Bool)

Initializes a new action for a call identified by a given UUID, as well as whether the call is muted.

init?(coder: NSCoder)

Creates a new action for a call with data in an unarchiver.

### Accessing Action Attributes

var isMuted: Bool

A Boolean value that indicates whether the call is muted.

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

### Call-related actions

class CXAction

An abstract class that declares a programmatic interface for objects that represent a telephony action.

class CXCallAction

A programmatic interface for objects that represent a telephony action associated with a call object.

class CXEndCallAction

An encapsulation of the act of ending a call.

class CXPlayDTMFCallAction

An encapsulation of the act of playing a dual tone multifrequency (DTMF) sequence.

class CXSetGroupCallAction

An encapsulation of the act of grouping or ungrouping calls.

class CXSetHeldCallAction

An encapsulation of the act of placing a call on hold or removing a call from hold.

