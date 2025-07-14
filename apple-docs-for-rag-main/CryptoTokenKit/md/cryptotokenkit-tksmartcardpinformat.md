

- CryptoTokenKit
-  TKSmartCardPINFormat 

Class

# TKSmartCardPINFormat

The formatting properties for a PIN, such as character encoding and length constraints.

iOSiPadOSMac Catalyst 13.1+macOS 10.11+tvOSvisionOSwatchOS

``` source
class TKSmartCardPINFormat
```

## Overview

You typically interact with `TKSmartCardPINFormat` objects when calling the userInteractionForSecurePINChange(_:apdu:currentPINByteOffset:newPINByteOffset:) and userInteractionForSecurePINVerification(_:apdu:pinByteOffset:) methods on an instance of TKSmartCard.

## Topics

### Configuring PIN Formatting

var charset: TKSmartCardPINFormat.Charset

The format of PIN characters. `TKSmartCardPINCharsetNumeric` by default.

var encoding: TKSmartCardPINFormat.Encoding

The encoding of PIN characters. `TKSmartCardPINEncodingASCII` by default.

var minPINLength: Int

The minimum number of characters to form a valid PIN. `4` by default.

var maxPINLength: Int

The maximum number of characters to form a valid PIN. `8` by default.

var pinBlockByteLength: Int

The total length of the PIN block in bytes. `8` by default.

var pinJustification: TKSmartCardPINFormat.Justification

The justification within the PIN block. `TKSmartCardPINJustificationLeft` by default.

var pinBitOffset: Int

The offset, in bits, within the PIN block to mark a location for filling in the formatted PIN, which is justified with respect to the pinJustification property value. `0` by default.

var pinLengthBitOffset: Int

The offset, in bits, within the PIN block to mark a location for filling in the PIN length, which is always left justified. `0` by default.

var pinLengthBitSize: Int

The size, in bits, of the PIN length field. If set to `0`, PIN length is not written. `0` by default.

### PIN Characteristics

enum Charset

Possible PIN character sets.

enum Encoding

Possible PIN encoding types.

enum Justification

Possible PIN justification types

## Relationships

### Inherits From

- NSObject

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

class TKSmartCardUserInteraction

The base class for encapsulating user interaction with a Smart Card reader.

class TKSmartCardUserInteractionForPINOperation

A representation of user interaction for secure PIN operations on a Smart Card reader.

class TKSmartCardUserInteractionForSecurePINChange

A representation of the user interaction for secure PIN change operations on a Smart Card reader.

class TKSmartCardUserInteractionForSecurePINVerification

A representation of the user interaction for secure PIN change verification on a Smart Card reader.

