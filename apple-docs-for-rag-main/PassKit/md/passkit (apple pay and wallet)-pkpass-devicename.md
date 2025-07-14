

- PassKit (Apple Pay and Wallet)
- PKPass
-  deviceName 

Instance Property

# deviceName

The name of the device that hosts the pass.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 11.0+visionOS 1.0+watchOS 3.0+

``` source
var deviceName: String { get }
```

## Discussion

If isRemotePass is true, this property contains the name of the paired device that stores the pass; otherwise, it contains the name of the device.

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

var localizedName: String

The localized name for the pass’s template.

var localizedDescription: String

The pass’s localized description.

var isRemotePass: Bool

A Boolean value that indicates whether the pass is on a paired device, such as an Apple Watch.

var paymentPass: PKPaymentPass?

The underlying payment pass.

Deprecated

