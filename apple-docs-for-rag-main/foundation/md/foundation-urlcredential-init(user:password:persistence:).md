

- Foundation
- URLCredential
-  init(user:password:persistence:) 

Initializer

# init(user:password:persistence:)

Creates a URL credential instance initialized with a given user name and password, using a given persistence setting.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
init(
    user: String,
    password: String,
    persistence: URLCredential.Persistence
)
```

## Parameters 

`user`  

The user for the credential.

`password`  

The password for `user`.

`persistence`  

A URLCredential.Persistence value indicating whether the credential should be stored permanently, for the duration of the current session, or not at all.

## Return Value

An instance of URLCredential, initialized with user name `user`, password `password`, and using persistence setting `persistence`.

## Discussion

If `persistence` is URLCredential.Persistence.permanent, the credential is stored in the keychain. If `persistence` is URLCredential.Persistence.synchronizable, it is also stored to the user’s other devices.

## See Also

### Creating a credential

init(forTrust: SecTrust)

Creates a URL credential instance for server trust authentication with a given accepted trust.

init(identity: SecIdentity, certificates: [Any]?, persistence: URLCredential.Persistence)

Creates a URL credential instance for resolving a client certificate authentication challenge.

init(trust: SecTrust)

Creates a URL credential instance for server trust authentication, initialized with a accepted trust.

enum Persistence

Constants that specify how long the credential will be kept.

