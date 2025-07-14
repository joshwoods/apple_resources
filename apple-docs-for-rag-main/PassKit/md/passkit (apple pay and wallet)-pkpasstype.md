

- PassKit (Apple Pay and Wallet)
-  PKPassType 

Enumeration

# PKPassType

Types of passes.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 11.0+visionOS 1.0+watchOS 3.0+

``` source
enum PKPassType
```

## Topics

### Pass types

case any

A nonspecific pass type.

case barcode

A pass that represents a barcode.

case secureElement

A pass that represents a credential that the device stores in the Secure Element.

static var payment: PKPassType

A pass that represents a credit or debit card

Deprecated

### Initializers

init?(rawValue: UInt)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Identifying a pass

var passType: PKPassType

The pass’s type.

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

var paymentPass: PKPaymentPass?

The underlying payment pass.

Deprecated

