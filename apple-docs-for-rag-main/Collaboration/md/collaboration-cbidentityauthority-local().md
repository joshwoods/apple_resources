

- Collaboration
- CBIdentityAuthority
-  local() 

Type Method

# local()

Returns the identity authority on the local system.

macOS 10.5+

``` source
class func local() -> CBIdentityAuthority
```

## Return Value

The identity authority on the local system.

## Discussion

Any identities stored on the local system are contained within this identity authority.

## See Also

### Accessing Identity Authorities

var localizedName: String

Returns the localized name of the identity authority.

class func managed() -> CBIdentityAuthority

Returns the identity authority that contains all the identities in bound network directory servers.

class func `default`() -> CBIdentityAuthority

Returns an identity authority that contains the identities in both the local and the network-bound authorities.

