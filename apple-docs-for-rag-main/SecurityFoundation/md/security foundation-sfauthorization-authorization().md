

- Security Foundation
- SFAuthorization
-  authorization() 

Type Method

# authorization()

Returns an authorization object initialized with a default environment, flags, and rights.

macOS 10.10+

``` source
class func authorization() -> Any!
```

## Return value

The authorization object.

## See Also

### Allocating and initializing an authorization object

class func authorization(with: AuthorizationFlags, rights: UnsafePointer&lt;AuthorizationRights>!, environment: UnsafePointer&lt;AuthorizationEnvironment>!) -> Any!

Returns an authorization object initialized with the specified flags, rights and environment.

init!()

Initializes an authorization object with default environment, flags, and rights.

init!(flags: AuthorizationFlags, rights: UnsafePointer&lt;AuthorizationRights>!, environment: UnsafePointer&lt;AuthorizationEnvironment>!)

Initializes an authorization object with the specified flags, rights, and environment.

