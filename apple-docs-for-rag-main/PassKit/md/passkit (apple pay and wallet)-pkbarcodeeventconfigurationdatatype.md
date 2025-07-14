

- PassKit (Apple Pay and Wallet)
-  PKBarcodeEventConfigurationDataType 

Enumeration

# PKBarcodeEventConfigurationDataType

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOSvisionOS 1.0+watchOS 7.0+

``` source
enum PKBarcodeEventConfigurationDataType
```

## Topics

### QR Code Purchase Signing Types

case signingCertificate

case signingKeyMaterial

case unknown

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Reading Configuration Information

var deviceAccountIdentifier: String

var configurationDataType: PKBarcodeEventConfigurationDataType

var configurationData: Data

