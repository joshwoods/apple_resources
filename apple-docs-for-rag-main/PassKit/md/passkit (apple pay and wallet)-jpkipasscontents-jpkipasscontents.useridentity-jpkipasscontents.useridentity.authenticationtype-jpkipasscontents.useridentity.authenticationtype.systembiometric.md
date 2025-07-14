

- PassKit (Apple Pay and Wallet)
- JPKIPassContents
- JPKIPassContents.UserIdentity
- JPKIPassContents.UserIdentity.AuthenticationType
-  JPKIPassContents.UserIdentity.AuthenticationType.systemBiometric 

Case

# JPKIPassContents.UserIdentity.AuthenticationType.systemBiometric

Authentication using biometric information.

iOS 18.0+iPadOS 18.0+

``` source
case systemBiometric
```

## Discussion

Use of the systemBiometric authentication requires you to set the NSFaceIDUsageDescription usage description.

## See Also

### Types of authentication

case pin(String)

The PIN associated with the user identity.

