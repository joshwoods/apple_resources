

- PassKit (Apple Pay and Wallet)
- PKShareablePassMetadata
-  init(provisioningCredentialIdentifier:cardConfigurationIdentifier:sharingInstanceIdentifier:passThumbnailImage:ownerDisplayName:localizedDescription:) Deprecated

Initializer

# init(provisioningCredentialIdentifier:cardConfigurationIdentifier:sharingInstanceIdentifier:passThumbnailImage:ownerDisplayName:localizedDescription:)

Creates a shareable pass metadata object.

iOS 14.0–16.0DeprecatediPadOS 14.0–16.0DeprecatedMac Catalyst 14.0–16.0DeprecatedmacOSvisionOS 1.0–1.0Deprecated

``` source
init?(
    provisioningCredentialIdentifier credentialIdentifier: String,
    cardConfigurationIdentifier: String,
    sharingInstanceIdentifier: String,
    passThumbnailImage: CGImage,
    ownerDisplayName: String,
    localizedDescription: String
)
```

Deprecated

Use initWithProvisioningCredentialIdentifier:sharingInstanceIdentifier:cardConfigurationIdentifier:passPreviewMetadata:

## Parameters 

`credentialIdentifier`  

A value that represents the user credentials for the pass.

`cardConfigurationIdentifier`  

A value that represents the configuration of the pass.

`sharingInstanceIdentifier`  

A unique value that you use to validate the shared pass.

`passThumbnailImage`  

A thumbnail image for the pass.

`ownerDisplayName`  

The name of the person that receives the shared pass.

`localizedDescription`  

A longer form of the pass description.

## See Also

### Creating a shareable pass metadata object

init(provisioningCredentialIdentifier: String, sharingInstanceIdentifier: String, passThumbnailImage: CGImage, ownerDisplayName: String, localizedDescription: String, accountHash: String, templateIdentifier: String, relyingPartyIdentifier: String, requiresUnifiedAccessCapableDevice: Bool)Deprecated

