

- Security
- AuthorizationFlags
-  destroyRights 

Type Property

# destroyRights

A flag that instructs the Security Server to revoke authorization.

Mac Catalyst 13.0+macOS 10.0+

``` source
static var destroyRights: AuthorizationFlags { get }
```

## Discussion

If this flag is set, the Security Server revokes authorization from the process as well as from any other process that is sharing the authorization. If not set, the Security Server revokes authorization from the process but not from other processes that share the authorization.

