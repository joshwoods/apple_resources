

- Security
-  kSecACLAuthorizationExportWrapped 

Global Variable

# kSecACLAuthorizationExportWrapped

Export a wrapped (that is, encrypted) key. This tag is checked on the key being exported; in addition, the `CSSM_ACL_AUTHORIZATION_ENCRYPT` tag is checked for any key used in the wrapping operation.

macOS 10.7+

``` source
let kSecACLAuthorizationExportWrapped: CFString
```

