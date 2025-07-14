

- CryptoTokenKit
-  TKSmartCardUserInteraction 

Class

# TKSmartCardUserInteraction

The base class for encapsulating user interaction with a Smart Card reader.

iOSiPadOSMac Catalyst 13.1+macOS 10.11+tvOSvisionOSwatchOS

``` source
class TKSmartCardUserInteraction
```

## Overview

There are two types of user interactions: those for secure PIN change and those for secure PIN validation. These interactions are instances of the TKSmartCardUserInteractionForSecurePINChange, or TKSmartCardUserInteractionForSecurePINVerification subclasses of TKSmartCardUserInteractionForPINOperation, respectively. TKSmartCardUserInteractionForPINOperation is a subclass of `TKSmartCardUserInteraction`.

You interact with instances of one of the subclasses of TKSmartCardUserInteractionForPINOperationwhen calling the userInteractionForSecurePINChange(_:apdu:currentPINByteOffset:newPINByteOffset:) and userInteractionForSecurePINVerification(_:apdu:pinByteOffset:) methods on an TKSmartCard object.

## Topics

### Handling User Interaction Events

var delegate: (any TKSmartCardUserInteractionDelegate)?

The delegate for observing events that occur during the user interaction.

protocol TKSmartCardUserInteractionDelegate

The interface implemented by a Smart Card user interaction delegate to handle user interaction events.

### Configuring Timeout

var initialTimeout: TimeInterval

The timeout, in seconds, for initial interaction. If set to `0`, the reader-defined default timeout is used. `0` by default.

var interactionTimeout: TimeInterval

The timeout, in seconds, after the first key stroke. If set to `0`, the reader-defined default timeout is used. `0` by default.

### Starting and Stopping

func run(reply: (Bool, (any Error)?) -> Void)

Runs the user interaction and asynchronously receives a reply.

func cancel() -> Bool

Attempts to cancel an interaction started by calling run(reply:). For certain interactions, cancellation may not be available.

## Relationships

### Inherits From

- NSObject

### Inherited By

- TKSmartCardUserInteractionForPINOperation

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

class TKSmartCardUserInteractionForPINOperation

A representation of user interaction for secure PIN operations on a Smart Card reader.

class TKSmartCardUserInteractionForSecurePINChange

A representation of the user interaction for secure PIN change operations on a Smart Card reader.

class TKSmartCardUserInteractionForSecurePINVerification

A representation of the user interaction for secure PIN change verification on a Smart Card reader.

