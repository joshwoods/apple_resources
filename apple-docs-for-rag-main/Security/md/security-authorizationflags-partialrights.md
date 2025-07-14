

- Security
- AuthorizationFlags
-  partialRights 

Type Property

# partialRights

A flag that permits the Security Server to grant rights on an individual basis.

Mac Catalyst 13.0+macOS 10.0+

``` source
static var partialRights: AuthorizationFlags { get }
```

## Discussion

If this and the extendRights flags are set, the Security Server grants or denies rights on an individual basis and all rights are checked.

