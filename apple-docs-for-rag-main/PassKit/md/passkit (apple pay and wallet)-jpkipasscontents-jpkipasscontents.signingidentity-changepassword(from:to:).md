

- PassKit (Apple Pay and Wallet)
- JPKIPassContents
- JPKIPassContents.SigningIdentity
-  changePassword(from:to:) 

Instance Method

# changePassword(from:to:)

A function that allows you to change the password associated with the signing identity.

iOS 18.0+iPadOS 18.0+

``` source
func changePassword(
    from oldValue: String,
    to newValue: String
) async throws
```

## Parameters 

`oldValue`  

The user authentication value used to perform the request to change the password.

`newValue`  

The new user authentication value applied to the signing identity.

## See Also

### Signing identity authentication

let signingIdentity: JPKIPassContents.SigningIdentity?

Allows access to the signing identity, if present in the JPKI applet.

enum AuthenticationType

Defines the valid user authentication request options for the signing identity.

