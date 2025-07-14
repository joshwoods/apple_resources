

- CallKit
-  CXCallAction 

Class

# CXCallAction

A programmatic interface for objects that represent a telephony action associated with a call object.

iOS 10.0+iPadOS 10.0+Mac Catalyst 10.0+visionOS 1.0+watchOS 9.0+

``` source
class CXCallAction
```

## Overview

The CallKit framework provides the following concrete CXCallAction subclasses.

| CXCallAction subclass | Description |
|----|----|
| CXAnswerCallAction | Answers an incoming call. |
| CXStartCallAction | Initiates an outgoing call. |
| CXEndCallAction | Ends a call. |
| CXSetHeldCallAction | Places a call on hold or removes a call from hold. |
| CXSetGroupCallAction | Groups a call with another call or removes a call from a group. |
| CXSetMutedCallAction | Mutes or unmutes a call. |
| CXPlayDTMFCallAction | Plays a DTMF (dual tone multifrequency) tone sequence on a call. |

To perform one or more actions, you add them to a new CXTransaction object and pass the transaction to an instance of CXCallController using the request(_:completion:) method. After each action is performed by the telephony provider, the provider’s delegate calls either the CXCallAction method, indicating that the action was successfully performed, or the CXCallAction method, to indicate that an error occurred; both of these methods set the CXCallAction property of the action to true.

## Topics

### Creating New Call Actions

init(call: UUID)

Initializes a new action for a call identified by a given UUID.

init?(coder: NSCoder)

Creates a new action for a call with data in an unarchiver.

### Accessing Call Action Attributes

var callUUID: UUID

The unique identifier for the call associated with the action.

## Relationships

### Inherits From

- CXAction

### Inherited By

- CXAnswerCallAction
- CXEndCallAction
- CXPlayDTMFCallAction
- CXSetGroupCallAction
- CXSetHeldCallAction
- CXSetMutedCallAction
- CXStartCallAction

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

class CXEndCallAction

An encapsulation of the act of ending a call.

class CXPlayDTMFCallAction

An encapsulation of the act of playing a dual tone multifrequency (DTMF) sequence.

class CXSetGroupCallAction

An encapsulation of the act of grouping or ungrouping calls.

class CXSetHeldCallAction

An encapsulation of the act of placing a call on hold or removing a call from hold.

class CXSetMutedCallAction

An encapsulation of the act of muting or unmuting a call.

