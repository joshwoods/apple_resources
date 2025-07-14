

- Authentication Services
- ASAuthorizationWebBrowserPlatformPublicKeyCredential
-  name 

Instance Property

# name

The user name for the account associated with this credential.

iOS 17.4+iPadOS 17.4+Mac Catalyst 16.4+macOS 13.3+

``` source
let name: String
```

## See Also

### Describing credentials

let customTitle: String

A string the person can supply to describe this credential.

let providerName: String

The name of the app that manages this credential, or “iCloud Keychain” if it’s the operating system.

let relyingParty: String

The relying party that issues challenges for this credential.

let userHandle: Data

A unique identifier for the user account at the relying party.

