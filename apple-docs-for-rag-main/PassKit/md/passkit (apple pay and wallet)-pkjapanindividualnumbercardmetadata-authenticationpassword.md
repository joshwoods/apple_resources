

- PassKit (Apple Pay and Wallet)
- PKJapanIndividualNumberCardMetadata
-  authenticationPassword 

Instance Property

# authenticationPassword

A string that specifies the authentication password when provisioning the pass.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOSvisionOS 2.0+

``` source
var authenticationPassword: String? { get set }
```

## See Also

### Defining configuration

var preview: PKAddPassMetadataPreview

An object that contains information representing the pass for provisioning.

var signingPassword: String?

A string that sets the signing password when you provision the pass.

