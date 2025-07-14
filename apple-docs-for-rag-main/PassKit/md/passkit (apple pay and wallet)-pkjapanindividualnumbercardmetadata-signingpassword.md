

- PassKit (Apple Pay and Wallet)
- PKJapanIndividualNumberCardMetadata
-  signingPassword 

Instance Property

# signingPassword

A string that sets the signing password when you provision the pass.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOSvisionOS 2.0+

``` source
var signingPassword: String? { get set }
```

## See Also

### Defining configuration

var authenticationPassword: String?

A string that specifies the authentication password when provisioning the pass.

var preview: PKAddPassMetadataPreview

An object that contains information representing the pass for provisioning.

