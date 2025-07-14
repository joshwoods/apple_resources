

- PassKit (Apple Pay and Wallet)
- JPKIPassContents
-  userIdentity 

Instance Property

# userIdentity

Allows for access to the user identity, if present in the JPKI applet.

iOS 18.0+iPadOS 18.0+

``` source
let userIdentity: JPKIPassContents.UserIdentity?
```

## See Also

### Identifying the pass user

func changePIN(from: String, to: String) async throws

A function that allows for the change of the PIN associated with the user identity.

enum AuthenticationType

Defines valid authentication types associated with the user identity.

