

- Collaboration
- CBIdentityAuthority
-  default() 

Type Method

# default()

Returns an identity authority that contains the identities in both the local and the network-bound authorities.

macOS 10.5+

``` source
class func `default`() -> CBIdentityAuthority
```

## Return Value

The local and network-bound identity authorities.

## Discussion

The default identity authority is the logical union of the identities in the local and managed authorities.

## See Also

### Accessing Identity Authorities

var localizedName: String

Returns the localized name of the identity authority.

class func local() -> CBIdentityAuthority

Returns the identity authority on the local system.

class func managed() -> CBIdentityAuthority

Returns the identity authority that contains all the identities in bound network directory servers.

