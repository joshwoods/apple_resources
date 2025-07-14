

- Authentication Services
- ASPasswordCredentialIdentity
-  init(serviceIdentifier:user:recordIdentifier:) 

Initializer

# init(serviceIdentifier:user:recordIdentifier:)

Initializes a password credential identity.

iOS 12.0+iPadOS 12.0+Mac Catalyst 14.0+macOS 11.0+visionOS 1.0+

``` source
init(
    serviceIdentifier: ASCredentialServiceIdentifier,
    user: String,
    recordIdentifier: String?
)
```

## Parameters 

`serviceIdentifier`  

The service identifier for the identity.

`user`  

The user associated with the identity.

`recordIdentifier`  

A string that your app can set to correlate the identity with an entry in your password database.

## See Also

### Creating a credential identity

class ASCredentialServiceIdentifier

An identifier representing a particular service for which the user needs a credential, like a web site.

