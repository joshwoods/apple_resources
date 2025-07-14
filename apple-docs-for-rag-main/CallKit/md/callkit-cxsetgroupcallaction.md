

- CallKit
-  CXSetGroupCallAction 

Class

# CXSetGroupCallAction

An encapsulation of the act of grouping or ungrouping calls.

iOS 10.0+iPadOS 10.0+Mac Catalyst 10.0+visionOS 1.0+watchOS 9.0+

``` source
class CXSetGroupCallAction
```

## Overview

CXSetGroupCallAction is a concrete subclass of CXCallAction. When the user or the system groups a call with another call, the provider sends provider(_:perform:) to its delegate. The provider’s delegate calls the fulfill() method to indicate that the action was successfully performed. A group call allows more than two recipients to simultaneously communicate with one another.

## Topics

### Creating New Actions

init(call: UUID, callUUIDToGroupWith: UUID?)

Initializes a new action for a call identified by a given UUID, as well as a call to group with identified by another UUID.

init?(coder: NSCoder)

Creates a new action to group calls with data in an unarchiver.

### Accessing Action Attributes

var callUUIDToGroupWith: UUID?

The unique identifier of the call to be grouped with the call associated with the receiver.

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

class CXSetHeldCallAction

An encapsulation of the act of placing a call on hold or removing a call from hold.

class CXSetMutedCallAction

An encapsulation of the act of muting or unmuting a call.

