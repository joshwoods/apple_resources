

- PassKit (Apple Pay and Wallet)
- PKPass
-  paymentPass Deprecated

Instance Property

# paymentPass

The underlying payment pass.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 11.0–15.4DeprecatedvisionOS 1.0–2.4DeprecatedwatchOS 3.0–9.0Deprecated

``` source
var paymentPass: PKPaymentPass? { get }
```

Deprecated

Use secureElementPass instead.

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

var localizedDescription: String

The pass’s localized description.

var isRemotePass: Bool

A Boolean value that indicates whether the pass is on a paired device, such as an Apple Watch.

