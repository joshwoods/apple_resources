

- PassKit (Apple Pay and Wallet)
- JPKIPassContents
-  signingIdentity 

Instance Property

# signingIdentity

Allows access to the signing identity, if present in the JPKI applet.

iOS 18.0+iPadOS 18.0+

``` source
let signingIdentity: JPKIPassContents.SigningIdentity?
```

## See Also

### Signing identity authentication

func changePassword(from: String, to: String) async throws

A function that allows you to change the password associated with the signing identity.

enum AuthenticationType

Defines the valid user authentication request options for the signing identity.

