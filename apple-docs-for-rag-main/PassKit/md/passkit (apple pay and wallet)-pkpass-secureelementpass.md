

- PassKit (Apple Pay and Wallet)
- PKPass
-  secureElementPass 

Instance Property

# secureElementPass

The pass that contains an accompanying credential that the device stores in the Secure Element.

iOS 13.4+iPadOS 13.4+Mac Catalyst 13.4+macOS 11.0+visionOS 1.0+watchOS 6.2+

``` source
var secureElementPass: PKSecureElementPass? { get }
```

## Discussion

Passes that contain sensitive information — for example, payment cards or digital car keys — store that information in the device’s Secure Element as an instance of PKSecureElementPass. Use this property to access the accompanying pass, which you can then use for other operations, such as signing data using a cryptographic signature.

## See Also

### Identifying a pass

var passType: PKPassType

The pass’s type.

enum PKPassType

Types of passes.

var serialNumber: String

A value that uniquely identifies the pass.

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

