

- CallKit
-  CXPlayDTMFCallAction 

Class

# CXPlayDTMFCallAction

An encapsulation of the act of playing a dual tone multifrequency (DTMF) sequence.

iOS 10.0+iPadOS 10.0+Mac Catalyst 10.0+visionOS 1.0+watchOS 9.0+

``` source
class CXPlayDTMFCallAction
```

## Overview

CXPlayDTMFCallAction is a concrete subclass of CXCallAction. Whenever digits are transmitted during a call, whether from a user interacting with a number pad or following a hard or soft pause, the provider sends provider(_:perform:) to its delegate. The provider’s delegate calls the fulfill() method to indicate that the action was successfully performed.

The provider sends provider(_:perform:) for successive actions only after the current action is fulfilled. When interacting with the number pad, each entered digit constitutes its own action. Digits following a hard or soft pause, however, are passed to provider(_:perform:) as a single string of digits. For example, if a user taps the 4 button on the number pad, followed by the 2 button, the delegate is sent provider(_:perform:) for the digit `4` and waits for the action to be fulfilled; after the action is fulfilled, the delegate is sent provider(_:perform:) for the digit `2`.

CallKit automatically plays the corresponding DTMF frequencies for any digits transmitted over a call. The app is responsible for managing the timing and handling of digits as part of fulfilling the action.

## Topics

### Creating New Actions

init(call: UUID, digits: String, type: CXPlayDTMFCallAction.ActionType)

Initializes a new action for a call identified by a given UUID, as well as a specified type and sequence of digits.

init?(coder: NSCoder)

Creates a new action to play dual-tone multifrequency (DTMF) tones with data in an unarchiver.

### Accessing Action Information

var digits: String

The digits tapped by the user into the in-call keypad or included in the dial string.

var type: CXPlayDTMFCallAction.ActionType

The type of the call action.

### Constants

enum ActionType

The types of events that generate dial tones.

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

class CXSetGroupCallAction

An encapsulation of the act of grouping or ungrouping calls.

class CXSetHeldCallAction

An encapsulation of the act of placing a call on hold or removing a call from hold.

class CXSetMutedCallAction

An encapsulation of the act of muting or unmuting a call.

