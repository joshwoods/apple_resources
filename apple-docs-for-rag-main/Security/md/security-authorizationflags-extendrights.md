

- Security
- AuthorizationFlags
-  extendRights 

Type Property

# extendRights

A flag that permits the Security Server to attempt to grant the rights requested.

Mac Catalyst 13.0+macOS 10.0+

``` source
static var extendRights: AuthorizationFlags { get }
```

## Discussion

Once the Security Server denies one right, it ignores the remaining requested rights.

