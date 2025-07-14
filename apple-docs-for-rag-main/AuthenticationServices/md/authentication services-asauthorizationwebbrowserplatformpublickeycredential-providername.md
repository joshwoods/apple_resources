

- Authentication Services
- ASAuthorizationWebBrowserPlatformPublicKeyCredential
-  providerName 

Instance Property

# providerName

The name of the app that manages this credential, or “iCloud Keychain” if it’s the operating system.

iOS 17.4+iPadOS 17.4+Mac Catalyst 16.4+macOS 13.3+

``` source
let providerName: String
```

## See Also

### Describing credentials

let customTitle: String

A string the person can supply to describe this credential.

let name: String

The user name for the account associated with this credential.

let relyingParty: String

The relying party that issues challenges for this credential.

let userHandle: Data

A unique identifier for the user account at the relying party.

