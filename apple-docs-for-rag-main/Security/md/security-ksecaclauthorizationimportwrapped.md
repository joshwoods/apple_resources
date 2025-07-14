

- Security
-  kSecACLAuthorizationImportWrapped 

Global Variable

# kSecACLAuthorizationImportWrapped

Import an encrypted key. This tag is checked on the key being imported; in addition, the `CSSM_ACL_AUTHORIZATION_DECRYPT` tag is checked for any key used in the unwrapping operation.

macOS 10.7+

``` source
let kSecACLAuthorizationImportWrapped: CFString
```

