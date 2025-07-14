

- CallKit
-  CXEndCallAction 

Class

# CXEndCallAction

An encapsulation of the act of ending a call.

iOS 10.0+iPadOS 10.0+Mac Catalyst 10.0+visionOS 1.0+watchOS 9.0+

``` source
class CXEndCallAction
```

## Overview

CXEndCallAction is a concrete subclass of CXCallAction. When the user initiates an outgoing call, the provider sends provider(_:perform:) to its delegate. The provider’s delegate calls the fulfill() method to indicate that the action was successfully performed. To indicate that the call ended at a time other than the current time, you can instead call the fulfill(withDateEnded:)

## Topics

### Completing Actions

func fulfill(withDateEnded: Date)

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

### Call-related actions

class CXAction

An abstract class that declares a programmatic interface for objects that represent a telephony action.

class CXCallAction

A programmatic interface for objects that represent a telephony action associated with a call object.

class CXPlayDTMFCallAction

An encapsulation of the act of playing a dual tone multifrequency (DTMF) sequence.

class CXSetGroupCallAction

An encapsulation of the act of grouping or ungrouping calls.

class CXSetHeldCallAction

An encapsulation of the act of placing a call on hold or removing a call from hold.

class CXSetMutedCallAction

An encapsulation of the act of muting or unmuting a call.

