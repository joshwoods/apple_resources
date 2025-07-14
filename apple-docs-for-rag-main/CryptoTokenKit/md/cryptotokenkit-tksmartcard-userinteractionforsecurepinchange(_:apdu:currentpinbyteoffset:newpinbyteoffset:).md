

- CryptoTokenKit
- TKSmartCard
-  userInteractionForSecurePINChange(\_:apdu:currentPINByteOffset:newPINByteOffset:) 

Instance Method

# userInteractionForSecurePINChange(\_:apdu:currentPINByteOffset:newPINByteOffset:)

Creates a new user interaction object for secure PIN change using the smart card reader facilities (typically a HW keypad).

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func userInteractionForSecurePINChange(
    _ PINFormat: TKSmartCardPINFormat,
    apdu APDU: Data,
    currentPINByteOffset: Int,
    newPINByteOffset: Int
) -> TKSmartCardUserInteractionForSecurePINChange?
```

## Parameters 

`PINFormat`  

The PIN format descriptor.

`APDU`  

The Application Protocol Data Unit (APDU) used by the Smart Card to fill in PIN data.

`currentPINByteOffset`  

The offset, in bytes, within the Application Protocol Data Unit (APDU) field to mark a location of a PIN block for filling in the entered PIN.

`newPINByteOffset`  

The offset, in bytes, within the Application Protocol Data Unit (APDU) field to mark a location of a PIN block for filling in the new PIN.

## Return Value

A new user interaction object for secure PIN verification, or `nil` if this feature is not supported by the Smart Card reader.

## Discussion

You should only call this method after a session to the Smart Card has been established using the beginSession(reply:) method, and before the session is terminated using the endSession() method.

Once the interaction has been successfully completed, the results are available via the resultData and resultSW properties of the returned TKSmartCardUserInteractionForSecurePINVerification object.

## See Also

### Managing User Interaction

func userInteractionForSecurePINVerification(TKSmartCardPINFormat, apdu: Data, pinByteOffset: Int) -> TKSmartCardUserInteractionForSecurePINVerification?

Creates and returns a new user interaction object for secure PIN verification using the Smart Card reader facilities.

class TKSmartCardPINFormat

The formatting properties for a PIN, such as character encoding and length constraints.

class TKSmartCardUserInteraction

The base class for encapsulating user interaction with a Smart Card reader.

class TKSmartCardUserInteractionForPINOperation

A representation of user interaction for secure PIN operations on a Smart Card reader.

class TKSmartCardUserInteractionForSecurePINChange

A representation of the user interaction for secure PIN change operations on a Smart Card reader.

class TKSmartCardUserInteractionForSecurePINVerification

A representation of the user interaction for secure PIN change verification on a Smart Card reader.

