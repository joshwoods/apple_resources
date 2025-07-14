

- PassKit (Apple Pay and Wallet)
- JPKIPassContents
- JPKIPassContents.UserIdentity
-  changePIN(from:to:) 

Instance Method

# changePIN(from:to:)

A function that allows for the change of the PIN associated with the user identity.

iOS 18.0+iPadOS 18.0+

``` source
func changePIN(
    from oldValue: String,
    to newValue: String
) async throws
```

## Parameters 

`oldValue`  

The user authentication value used to perform the request to change the PIN.

`newValue`  

The new user authentication value applied to user identity.

## See Also

### Identifying the pass user

let userIdentity: JPKIPassContents.UserIdentity?

Allows for access to the user identity, if present in the JPKI applet.

enum AuthenticationType

Defines valid authentication types associated with the user identity.

