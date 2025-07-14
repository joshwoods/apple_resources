

- PassKit (Apple Pay and Wallet)
- JPKIPassContents
- JPKIPassContents.SigningIdentity
-  JPKIPassContents.SigningIdentity.AuthenticationType 

Enumeration

# JPKIPassContents.SigningIdentity.AuthenticationType

Defines the valid user authentication request options for the signing identity.

iOS 18.0+iPadOS 18.0+

``` source
enum AuthenticationType
```

## Topics

### Case for authentication

case password(String)

Reads the signing identity using the password.

## See Also

### Signing identity authentication

let signingIdentity: JPKIPassContents.SigningIdentity?

Allows access to the signing identity, if present in the JPKI applet.

func changePassword(from: String, to: String) async throws

A function that allows you to change the password associated with the signing identity.

