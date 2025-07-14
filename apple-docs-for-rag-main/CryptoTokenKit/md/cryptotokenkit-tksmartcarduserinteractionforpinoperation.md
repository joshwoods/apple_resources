

- CryptoTokenKit
-  TKSmartCardUserInteractionForPINOperation 

Class

# TKSmartCardUserInteractionForPINOperation

A representation of user interaction for secure PIN operations on a Smart Card reader.

iOSiPadOSMac Catalyst 13.1+macOS 10.11+tvOSvisionOSwatchOS

``` source
class TKSmartCardUserInteractionForPINOperation
```

## Overview

There are two types of user interactions: those for secure PIN change and those for secure PIN validation. These interactions are instances of the TKSmartCardUserInteractionForSecurePINChange, or TKSmartCardUserInteractionForSecurePINVerification subclasses of TKSmartCardUserInteractionForPINOperation, respectively.

You interact with instances of one of the subclasses of TKSmartCardUserInteractionForPINOperation when calling the userInteractionForSecurePINChange(_:apdu:currentPINByteOffset:newPINByteOffset:) and userInteractionForSecurePINVerification(_:apdu:pinByteOffset:) methods on an TKSmartCard object.

The result of a user interaction is available once the interaction has completed.

## Topics

### Managing Pin Completion

var pinCompletion: TKSmartCardUserInteractionForPINOperation.Completion

The conditions under which PIN entry should be considered complete.

struct Completion

### Configuring Messages

var pinMessageIndices: [NSNumber]?

A list of message indices referring to a predefined message table, used to specify the type and number of messages displayed during the PIN operation. `nil` by default.

var locale: Locale!

The locale for the displayed messages. If `nil`, the user’s current locale is used. By default, this value is the current locale of the system.

### Accessing Response Data

var resultSW: UInt16

The SW1-SW2 status bytes.

var resultData: Data?

The returned data without SW1-SW2 bytes, if any.

## Relationships

### Inherits From

- TKSmartCardUserInteraction

### Inherited By

- TKSmartCardUserInteractionForSecurePINChange
- TKSmartCardUserInteractionForSecurePINVerification

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Managing User Interaction

func userInteractionForSecurePINVerification(TKSmartCardPINFormat, apdu: Data, pinByteOffset: Int) -> TKSmartCardUserInteractionForSecurePINVerification?

Creates and returns a new user interaction object for secure PIN verification using the Smart Card reader facilities.

func userInteractionForSecurePINChange(TKSmartCardPINFormat, apdu: Data, currentPINByteOffset: Int, newPINByteOffset: Int) -> TKSmartCardUserInteractionForSecurePINChange?

Creates a new user interaction object for secure PIN change using the smart card reader facilities (typically a HW keypad).

class TKSmartCardPINFormat

The formatting properties for a PIN, such as character encoding and length constraints.

class TKSmartCardUserInteraction

The base class for encapsulating user interaction with a Smart Card reader.

class TKSmartCardUserInteractionForSecurePINChange

A representation of the user interaction for secure PIN change operations on a Smart Card reader.

class TKSmartCardUserInteractionForSecurePINVerification

A representation of the user interaction for secure PIN change verification on a Smart Card reader.

