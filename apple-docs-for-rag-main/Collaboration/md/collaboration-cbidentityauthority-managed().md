

- Collaboration
- CBIdentityAuthority
-  managed() 

Type Method

# managed()

Returns the identity authority that contains all the identities in bound network directory servers.

macOS 10.5+

``` source
class func managed() -> CBIdentityAuthority
```

## Return Value

The identity authorities in bound network directory servers.

## Discussion

If you are bound to a network directory server (such as an LDAP server) that has an identity authority, use this method to search those authorities.

## See Also

### Accessing Identity Authorities

var localizedName: String

Returns the localized name of the identity authority.

class func local() -> CBIdentityAuthority

Returns the identity authority on the local system.

class func `default`() -> CBIdentityAuthority

Returns an identity authority that contains the identities in both the local and the network-bound authorities.

