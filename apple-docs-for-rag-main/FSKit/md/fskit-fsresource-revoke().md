

- FSKit
- FSResource
-  revoke() 

Instance Method

# revoke()

Revokes the resource.

macOS 15.4+

``` source
func revoke()
```

## Discussion

This method works by stripping away any underlying privileges associated with the resource. This effectively disconnects this object from its underlying resource.

## See Also

### Revoking the resource

var isRevoked: Bool

A Boolean value that indicates whether the resource is revoked.

