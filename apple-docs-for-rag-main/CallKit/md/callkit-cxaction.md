

- CallKit
-  CXAction 

Class

# CXAction

An abstract class that declares a programmatic interface for objects that represent a telephony action.

iOS 10.0+iPadOS 10.0+Mac Catalyst 10.0+visionOS 1.0+watchOS 9.0+

``` source
class CXAction
```

## Overview

Each instance of CXAction is uniquely identified by a uuid, which is generated on initialization. An action also tracks whether it has been completed or not.

To perform one or more actions, you add them to a new CXTransaction object and pass the transaction to an instance of CXCallController using the request(_:completion:) method. After each action is performed by the telephony provider, the provider’s delegate calls either the fulfill() method, indicating that the action was successfully performed, or the fail() method, to indicate that an error occurred; both of these methods set the isComplete property of the action to true.

The CXCallAction subclass is an abstract class that represents an action associated with a CXCall object. The CallKit framework provides several concrete CXCallAction subclasses to represent actions such as answering a call and putting a call on hold.

## Topics

### Creating an Action

init()

Initializes a new telephony action.

init?(coder: NSCoder)

Creates a new telephony action with data in an unarchiver.

### Accessing Action Attributes

var uuid: UUID

The unique identifier for the action.

var isComplete: Bool

A Boolean value that indicates whether the action has been performed by the provider.

var timeoutDate: Date

The time after which the action cannot be completed.

### Completing Actions

func fulfill()

Reports the successful execution of the action.

func fail()

Reports the failed execution of the action.

## Relationships

### Inherits From

- NSObject

### Inherited By

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

class CXSetMutedCallAction

An encapsulation of the act of muting or unmuting a call.

