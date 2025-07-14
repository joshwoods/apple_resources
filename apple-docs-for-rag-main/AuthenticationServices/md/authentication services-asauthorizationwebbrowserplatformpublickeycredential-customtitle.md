

- Authentication Services
- ASAuthorizationWebBrowserPlatformPublicKeyCredential
-  customTitle 

Instance Property

# customTitle

A string the person can supply to describe this credential.

iOS 17.4+iPadOS 17.4+Mac Catalyst 17.0+macOS 14.0+

``` source
let customTitle: String
```

## See Also

### Describing credentials

let name: String

The user name for the account associated with this credential.

let providerName: String

The name of the app that manages this credential, or “iCloud Keychain” if it’s the operating system.

let relyingParty: String

The relying party that issues challenges for this credential.

let userHandle: Data

A unique identifier for the user account at the relying party.

