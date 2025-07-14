

- Security Foundation
- SFAuthorization
-  init() 

Initializer

# init()

Initializes an authorization object with default environment, flags, and rights.

macOS 10.10+

``` source
init!()
```

## See Also

### Allocating and initializing an authorization object

class func authorization() -> Any!

Returns an authorization object initialized with a default environment, flags, and rights.

class func authorization(with: AuthorizationFlags, rights: UnsafePointer&lt;AuthorizationRights>!, environment: UnsafePointer&lt;AuthorizationEnvironment>!) -> Any!

Returns an authorization object initialized with the specified flags, rights and environment.

init!(flags: AuthorizationFlags, rights: UnsafePointer&lt;AuthorizationRights>!, environment: UnsafePointer&lt;AuthorizationEnvironment>!)

Initializes an authorization object with the specified flags, rights, and environment.

