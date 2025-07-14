

- Security Foundation
- SFAuthorization
-  authorization(with:rights:environment:) 

Type Method

# authorization(with:rights:environment:)

Returns an authorization object initialized with the specified flags, rights and environment.

macOS 10.10+

``` source
class func authorization(
    with flags: AuthorizationFlags,
    rights: UnsafePointer!,
    environment: UnsafePointer!
) -> Any!
```

## Parameters 

`flags`  

A bit mask for specifying authorization options. Use the following option sets:

- Pass the constant kAuthorizationFlagDefaults if no options are necessary.

- Specify the extendRights mask to request rights. You can also specify the interactionAllowed mask to allow user interaction.

- Specify the partialRights and extendRights masks to request partial rights. You can also specify the interactionAllowed mask to allow user interaction.

- Specify the preAuthorize and extendRights masks to preauthorize rights.

- Specify the destroyRights mask to prevent the Security framework from preserving the rights obtained during this call.

`rights`  

A pointer to a set of authorization rights you create. Pass `NULL` if the application requires no rights at this time.

`environment`  

Data used when authorizing or preauthorizing rights. In macOS 10.3 and later, you can pass icon or prompt data to be used in the authentication dialog box. Possible values for this parameter are listed in `Security.framework/Headers/AuthorizationTags.h`. The data passed in this parameter is not stored in the authorization reference; it is used only during authorization. If you are not passing any data in this parameter, pass the constant kAuthorizationEmptyEnvironment.

## Return value

The authorization object.

## Discussion

Normally, such initialization is not required, as you pass in flags, rights, and environmental data when you request authorization.

## See Also

### Allocating and initializing an authorization object

class func authorization() -> Any!

Returns an authorization object initialized with a default environment, flags, and rights.

init!()

Initializes an authorization object with default environment, flags, and rights.

init!(flags: AuthorizationFlags, rights: UnsafePointer&lt;AuthorizationRights>!, environment: UnsafePointer&lt;AuthorizationEnvironment>!)

Initializes an authorization object with the specified flags, rights, and environment.

