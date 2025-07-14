

- CryptoTokenKit
- TKTokenSmartCardPINAuthOperation
-  pinByteOffset 

Instance Property

# pinByteOffset

The offset, in bytes, within the APDU template to mark the location for filling in the PIN.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
var pinByteOffset: Int { get set }
```

## See Also

### Configuring the Operation

var pinFormat: TKSmartCardPINFormat

The PIN format.

var apduTemplate: Data?

The template into which the PIN is filled in. `nil` by default.

var smartCard: TKSmartCard?

A Smart Card to which the formatted APDU is sent in order to authenticate.

