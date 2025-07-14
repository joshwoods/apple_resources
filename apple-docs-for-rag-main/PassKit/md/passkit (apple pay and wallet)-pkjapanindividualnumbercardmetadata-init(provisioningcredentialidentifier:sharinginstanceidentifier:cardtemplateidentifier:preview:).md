

- PassKit (Apple Pay and Wallet)
- PKJapanIndividualNumberCardMetadata
-  init(provisioningCredentialIdentifier:sharingInstanceIdentifier:cardTemplateIdentifier:preview:) 

Initializer

# init(provisioningCredentialIdentifier:sharingInstanceIdentifier:cardTemplateIdentifier:preview:)

Initializes the product instance to provision.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOSvisionOS 2.0+

``` source
init(
    provisioningCredentialIdentifier credentialIdentifier: String,
    sharingInstanceIdentifier: String,
    cardTemplateIdentifier templateIdentifier: String,
    preview: PKAddPassMetadataPreview
)
```

## See Also

### Initializing the digital card metadata

init(provisioningCredentialIdentifier: String, sharingInstanceIdentifier: String, cardConfigurationIdentifier: String, preview: PKAddPassMetadataPreview)

Initializes the user instance for provisioning.

