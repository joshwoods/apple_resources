

- PassKit (Apple Pay and Wallet)
- PKPass
-  localizedDescription 

Instance Property

# localizedDescription

The pass’s localized description.

iOSiPadOSMac CatalystmacOSvisionOSwatchOS

``` source
var localizedDescription: String { get }
```

## Discussion

This property provides access to the description string from the pass’s JSON file. For more information about the JSON format, see Pass Design and Creation in Wallet Developer Guide. For information about adding localized strings to the JSON file, see Passes Support Localization in that same guide.

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

var localizedName: String

The localized name for the pass’s template.

var isRemotePass: Bool

A Boolean value that indicates whether the pass is on a paired device, such as an Apple Watch.

var paymentPass: PKPaymentPass?

The underlying payment pass.

Deprecated

