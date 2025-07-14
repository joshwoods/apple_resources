

- PassKit (Apple Pay and Wallet)
- PKPass
-  localizedName 

Instance Property

# localizedName

The localized name for the pass’s template.

iOSiPadOSMac CatalystmacOSvisionOSwatchOS

``` source
var localizedName: String { get }
```

## Discussion

The pass’s template defines the pass’s basic layout. For more information about the available templates, see Pass Style Sets the Overall Visual Appearance in Wallet Developer Guide.

## See Also

### Identifying a pass

var passType: PKPassType

The pass’s type.

enum PKPassType

Types of passes.

var secureElementPass: PKSecureElementPass?

The pass that contains an accompanying credential that the device stores in the Secure Element.

var serialNumber: String

A value that uniquely identifies the pass.

var passTypeIdentifier: String

The pass’s pass type identifier.

var deviceName: String

The name of the device that hosts the pass.

var localizedDescription: String

The pass’s localized description.

var isRemotePass: Bool

A Boolean value that indicates whether the pass is on a paired device, such as an Apple Watch.

var paymentPass: PKPaymentPass?

The underlying payment pass.

Deprecated

