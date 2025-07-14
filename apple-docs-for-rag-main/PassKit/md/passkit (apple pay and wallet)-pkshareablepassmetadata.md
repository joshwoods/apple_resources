

- PassKit (Apple Pay and Wallet)
-  PKShareablePassMetadata 

Class

# PKShareablePassMetadata

Information that you use to configure the sharing sheet for a pass.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOSvisionOS 1.0+

``` source
class PKShareablePassMetadata
```

## Topics

### Creating a shareable pass metadata object

init?(provisioningCredentialIdentifier: String, cardConfigurationIdentifier: String, sharingInstanceIdentifier: String, passThumbnailImage: CGImage, ownerDisplayName: String, localizedDescription: String)

Creates a shareable pass metadata object.

Deprecated

init(provisioningCredentialIdentifier: String, sharingInstanceIdentifier: String, passThumbnailImage: CGImage, ownerDisplayName: String, localizedDescription: String, accountHash: String, templateIdentifier: String, relyingPartyIdentifier: String, requiresUnifiedAccessCapableDevice: Bool)Deprecated

### Displaying information on the share sheet

var ownerDisplayName: String

The name of the person that receives a shared pass.

var passThumbnailImage: CGImage

A thumbnail image of a pass that the system displays on the sharing sheet.

var localizedDescription: String

A longer form of the pass description that the system displays on the sharing sheet.

### Reading notification properties

var accountHash: String

An Apple Push Notification push token.

var relyingPartyIdentifier: String

An identifier used in push notifications.

var templateIdentifier: String

An identifier used in push notifications.

var cardTemplateIdentifier: String

### Requiring a unified access capable device

var requiresUnifiedAccessCapableDevice: Bool

### Initializers

init(provisioningCredentialIdentifier: String, sharingInstanceIdentifier: String, cardConfigurationIdentifier: String, preview: PKShareablePassMetadata.Preview)

init(provisioningCredentialIdentifier: String, sharingInstanceIdentifier: String, cardTemplateIdentifier: String, preview: PKShareablePassMetadata.Preview)

### Instance Properties

var cardConfigurationIdentifier: String

A developer-defined value that represents the configuration of a pass.

var credentialIdentifier: String

A developer-defined value that represents the user credentials of a pass.

var preview: PKShareablePassMetadata.Preview

var serverEnvironmentIdentifier: String

var sharingInstanceIdentifier: String

A developer-defined unique value that you use to validate a shared pass.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Shareable passes

class PKAddShareablePassConfiguration

An object that represents the data and action for a shared copy of pass.

enum PKAddShareablePassConfigurationPrimaryAction

The kind of add action that the system performs with a pass.

