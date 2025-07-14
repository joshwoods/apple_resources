

- FSKit
- FSResource
-  isRevoked 

Instance Property

# isRevoked

A Boolean value that indicates whether the resource is revoked.

macOS 15.4+

``` source
var isRevoked: Bool { get }
```

## Discussion

If this is a proxy resource, the value of this property is always `true` (Swift) or `YES` (Objective-C).

## See Also

### Revoking the resource

func revoke()

Revokes the resource.

