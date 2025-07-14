

- PassKit (Apple Pay and Wallet)
- JPKIPassContents
- JPKIPassContents.AuthenticationRequest
-  init(type:) 

Initializer

# init(type:)

Initializes the user authentication request options for the signing identity type.

iOS 18.0+iPadOS 18.0+

``` source
init(type: JPKIPassContents.SigningIdentity.AuthenticationType)
```

Available when `IdentityType` is `JPKIPassContents.SigningIdentity`.

## See Also

### Creating authentication request options

init(type: JPKIPassContents.UserIdentity.AuthenticationType)

Initializes the user authentication request options for the user identity type.

