

- Security
-  AuthorizationCopyRightsAsync(\_:\_:\_:\_:\_:) 

Function

# AuthorizationCopyRightsAsync(\_:\_:\_:\_:\_:)

Authorizes and preauthorizes rights asynchronously.

Mac Catalyst 13.0+macOS 10.7+

``` source
func AuthorizationCopyRightsAsync(
    _ authorization: AuthorizationRef,
    _ rights: UnsafePointer,
    _ environment: UnsafePointer?,
    _ flags: AuthorizationFlags,
    _ callbackBlock: @escaping AuthorizationAsyncCallback
)
```

## Parameters 

`authorization`  

An authorization reference referring to the authorization session.

`rights`  

A pointer to a set of authorization rights you create. Pass `nil` if the application requires no rights at this time.

`environment`  

Data used when authorizing or preauthorizing rights. Not used in OS X v10.2 and earlier. In macOS 10.3 and later, you can pass icon or prompt data to be used in the authentication dialog box. In macOS 10.4 and later, you can also pass a user name and password in order to authorize a user without displaying the authentication dialog box. Possible values for this parameter are listed in `Security.framework/Headers/AuthorizationTags.h`. The data passed in this parameter is not stored in the authorization reference; it is used only during authorization. If you are not passing any data in this parameter, pass the constant kAuthorizationEmptyEnvironment.

`flags`  

A bit mask for specifying authorization options. Use one of the options sets defined for the flags parameter in the AuthorizationCopyRights(_:_:_:_:_:) function.

`callbackBlock`  

A callback that you provide for the function to call when it finishes asynchronously. Use a function with the signature defined by AuthorizationAsyncCallback.

## Discussion

See the discussion for AuthorizationCopyRights(_:_:_:_:_:). This function behaves similarly, except that it performs its operations asynchronously and calls back to you upon completion.

