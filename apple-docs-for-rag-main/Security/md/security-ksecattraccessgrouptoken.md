

- Security
-  kSecAttrAccessGroupToken 

Global Variable

# kSecAttrAccessGroupToken

The access group containing items provided by external tokens.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
let kSecAttrAccessGroupToken: CFString
```

## Discussion

Use this access group identifier as the value for the kSecAttrAccessGroup attribute in a keychain query to access external tokens such as smart cards. Access to this group is granted by default and does not require an explicit entry in your app’s Keychain Access Groups Entitlement.

