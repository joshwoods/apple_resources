

- CallKit
-  CXSetHeldCallAction 

Class

# CXSetHeldCallAction

An encapsulation of the act of placing a call on hold or removing a call from hold.

iOS 10.0+iPadOS 10.0+Mac Catalyst 10.0+visionOS 1.0+watchOS 9.0+

``` source
class CXSetHeldCallAction
```

## Overview

CXSetHeldCallAction is a concrete subclass of CXCallAction.

When a caller places a call on hold, callers are unable to communicate with one another until the holding caller removes the call from hold. Placing a call on hold doesn’t end the call.

When the user or the system places a call on hold, the provider sends provider(_:perform:) to its delegate. The provider’s delegate calls the fulfill() method to indicate that the action was successfully performed.

## Topics

### Creating New Actions

init(call: UUID, onHold: Bool)

Initializes a new action for a call identified by a given UUID, as well as whether the call is on hold.

init?(coder: NSCoder)

Creates a new action to place a call on hold with data in an unarchiver.

### Accessing Action Information

var isOnHold: Bool

A Boolean value that indicates whether the call is placed on hold.

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

class CXSetMutedCallAction

An encapsulation of the act of muting or unmuting a call.

