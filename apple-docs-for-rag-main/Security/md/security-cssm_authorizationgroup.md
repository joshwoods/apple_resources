

- Security
-  cssm_authorizationgroup 

Structure

# cssm_authorizationgroup

Mac Catalyst 13.0+macOS 10.0+

``` source
struct cssm_authorizationgroup
```

## Topics

### Initializers

init()

init(NumberOfAuthTags: uint32, AuthTags: UnsafeMutablePointer&lt;CSSM_ACL_AUTHORIZATION_TAG>!)

### Instance Properties

var AuthTags: UnsafeMutablePointer&lt;CSSM_ACL_AUTHORIZATION_TAG>!

var NumberOfAuthTags: uint32

## Relationships

### Conforms To

- BitwiseCopyable

