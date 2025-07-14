

- Collaboration
- CBIdentityAuthority
-  localizedName 

Instance Property

# localizedName

Returns the localized name of the identity authority.

macOS 10.5+

``` source
var localizedName: String { get }
```

## Return Value

The computer’s name if the authority is local, or Managed Network Directory if the authority is managed.

## See Also

### Accessing Identity Authorities

class func local() -> CBIdentityAuthority

Returns the identity authority on the local system.

class func managed() -> CBIdentityAuthority

Returns the identity authority that contains all the identities in bound network directory servers.

class func `default`() -> CBIdentityAuthority

Returns an identity authority that contains the identities in both the local and the network-bound authorities.

