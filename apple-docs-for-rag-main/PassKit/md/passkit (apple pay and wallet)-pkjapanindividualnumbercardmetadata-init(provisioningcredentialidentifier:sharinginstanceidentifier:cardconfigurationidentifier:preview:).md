

- PassKit (Apple Pay and Wallet)
- PKJapanIndividualNumberCardMetadata
-  init(provisioningCredentialIdentifier:sharingInstanceIdentifier:cardConfigurationIdentifier:preview:) 

Initializer

# init(provisioningCredentialIdentifier:sharingInstanceIdentifier:cardConfigurationIdentifier:preview:)

Initializes the user instance for provisioning.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOSvisionOS 2.0+

``` source
init(
    provisioningCredentialIdentifier credentialIdentifier: String,
    sharingInstanceIdentifier: String,
    cardConfigurationIdentifier templateIdentifier: String,
    preview: PKAddPassMetadataPreview
)
```

## Parameters 

`credentialIdentifier`  

An identifier for the user instance to provision.

`sharingInstanceIdentifier`  

A short-lived token to prevent replayability.

`templateIdentifier`  

An identifier for a legacy product on Apple Pay servers.

`preview`  

An object that contains information representing the provisioned pass in UI.

## See Also

### Initializing the digital card metadata

init(provisioningCredentialIdentifier: String, sharingInstanceIdentifier: String, cardTemplateIdentifier: String, preview: PKAddPassMetadataPreview)

Initializes the product instance to provision.

