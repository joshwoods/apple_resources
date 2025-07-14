

- PassKit (Apple Pay and Wallet)
- PKShareablePassMetadata
-  init(provisioningCredentialIdentifier:sharingInstanceIdentifier:passThumbnailImage:ownerDisplayName:localizedDescription:accountHash:templateIdentifier:relyingPartyIdentifier:requiresUnifiedAccessCapableDevice:) Deprecated

Initializer

# init(provisioningCredentialIdentifier:sharingInstanceIdentifier:passThumbnailImage:ownerDisplayName:localizedDescription:accountHash:templateIdentifier:relyingPartyIdentifier:requiresUnifiedAccessCapableDevice:)

iOS 15.0–16.0DeprecatediPadOS 15.0–16.0DeprecatedMac Catalyst 15.0–16.0DeprecatedmacOSvisionOS 1.0–1.0Deprecated

``` source
init(
    provisioningCredentialIdentifier credentialIdentifier: String,
    sharingInstanceIdentifier: String,
    passThumbnailImage: CGImage,
    ownerDisplayName: String,
    localizedDescription: String,
    accountHash: String,
    templateIdentifier: String,
    relyingPartyIdentifier: String,
    requiresUnifiedAccessCapableDevice: Bool
)
```

Deprecated

Use initWithProvisioningCredentialIdentifier:sharingInstanceIdentifier:cardTemplateIdentifier:passPreviewMetadata:

## See Also

### Creating a shareable pass metadata object

init?(provisioningCredentialIdentifier: String, cardConfigurationIdentifier: String, sharingInstanceIdentifier: String, passThumbnailImage: CGImage, ownerDisplayName: String, localizedDescription: String)

Creates a shareable pass metadata object.

Deprecated

