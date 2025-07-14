

- Matter
-  MTRSetupPayload 

Class

# MTRSetupPayload

iOS 16.1+iPadOS 16.1+Mac Catalyst 16.1+macOS 13.0+tvOS 16.1+visionOS 1.0+watchOS 9.1+

``` source
class MTRSetupPayload
```

## Mentioned in 

Onboarding a Matter device

## Topics

### Initializers

init(onboardingPayload: String) throwsDeprecated

init?(payload: String)

init(setupPasscode: NSNumber, discriminator: NSNumber)

### Instance Properties

var commissioningFlow: MTRCommissioningFlow

var discoveryCapabilities: MTRDiscoveryCapabilities

var discriminator: NSNumber

var hasShortDiscriminator: Bool

var productID: NSNumber

var rendezvousInformation: NSNumber?Deprecated

var serialNumber: String?

var setUpPINCode: NSNumberDeprecated

var setupPasscode: NSNumber

var vendorElements: [MTROptionalQRCodeInfo]

var vendorID: NSNumber

var version: NSNumber

### Instance Methods

func addOrReplaceVendorElement(MTROptionalQRCodeInfo)

func getAllOptionalVendorData() throws -> [MTROptionalQRCodeInfo]Deprecated

func manualEntryCode() -> String?

func qrCodeString() -> String?

func qrCodeString(NSErrorPointer) -> String?Deprecated

func removeVendorElement(withTag: NSNumber)

func vendorElement(withTag: NSNumber) -> MTROptionalQRCodeInfo?

### Type Methods

class func generateRandomPIN() -> IntDeprecated

class func generateRandomSetupPasscode() -> NSNumber

class func new() -> SelfDeprecated

class func isValidSetupPasscode(NSNumber) -> Bool

Check whether the provided setup passcode (represented as an unsigned integer) is a valid setup passcode.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- Copyable
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSCopying
- NSObjectProtocol
- NSSecureCoding

