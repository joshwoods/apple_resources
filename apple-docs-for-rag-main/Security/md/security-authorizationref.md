

- Security
-  AuthorizationRef 

Type Alias

# AuthorizationRef

A pointer to an opaque authorization reference structure.

Mac Catalyst 13.0+macOS 10.0+

``` source
typealias AuthorizationRef = OpaquePointer
```

## Discussion

This data type points to a structure the Security Server uses to store information about the authorization session. Use the functions described in Authorization Services to create, access, and free the authorization reference.

