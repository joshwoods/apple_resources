

- PassKit (Apple Pay and Wallet)
- PKPass
-  serialNumber 

Instance Property

# serialNumber

A value that uniquely identifies the pass.

iOSiPadOSMac CatalystmacOSvisionOSwatchOS

``` source
var serialNumber: String { get }
```

## See Also

### Identifying a pass

var passType: PKPassType

The pass’s type.

enum PKPassType

Types of passes.

var secureElementPass: PKSecureElementPass?

The pass that contains an accompanying credential that the device stores in the Secure Element.

var passTypeIdentifier: String

The pass’s pass type identifier.

var deviceName: String

The name of the device that hosts the pass.

var localizedName: String

The localized name for the pass’s template.

var localizedDescription: String

The pass’s localized description.

var isRemotePass: Bool

A Boolean value that indicates whether the pass is on a paired device, such as an Apple Watch.

var paymentPass: PKPaymentPass?

The underlying payment pass.

Deprecated

