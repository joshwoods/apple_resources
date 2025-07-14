

- Security
-  AuthorizationCreate(\_:\_:\_:\_:) 

Function

# AuthorizationCreate(\_:\_:\_:\_:)

Creates a new authorization reference and provides an option to authorize or preauthorize rights.

Mac Catalyst 13.0+macOS 10.0+

``` source
func AuthorizationCreate(
    _ rights: UnsafePointer?,
    _ environment: UnsafePointer?,
    _ flags: AuthorizationFlags,
    _ authorization: UnsafeMutablePointer?
) -> OSStatus
```

## Parameters 

`rights`  

A pointer to a set of authorization rights you create. Pass `nil` if the application requires no rights at this time.

`environment`  

An AuthorizationItemSet structure used when authorizing or preauthorizing rights. Not used in OS X v10.2 and earlier. In macOS 10.3 and later, you can pass icon or prompt data to be used in the authentication dialog box. In macOS 10.4 and later, you can also pass a user name and password in order to authorize a user without user interaction. Possible values for this parameter are listed in `Security.framework/Headers/AuthorizationTags.h`. The data passed in this parameter is not stored in the authorization reference; it is used only during authorization. If you are not passing any data in this parameter, pass the constant kAuthorizationEmptyEnvironment. For a list of possible keys in the authorization set, see Authorization Name Tags. For the data structure itself, see AuthorizationItemSet.

`flags`  

A bit mask constructed at the bitwise `OR` of one or more AuthorizationFlags for specifying authorization options. Use one of the following option sets:

- Use the constant kAuthorizationFlagDefaults if no options are necessary.

- Use the extendRights flag to request rights. You can also add the interactionAllowed flag to allow user interaction.

- Specify the partialRights and extendRights flags to request partial rights. You can also add the interactionAllowed flag to allow user interaction.

- Specify the preAuthorize and extendRights flags to preauthorize rights.

- Specify the destroyRights flag to prevent the Security Server from preserving the rights obtained during this call.

`authorization`  

A pointer to an authorization reference. On return, this parameter refers to the authorization session the Security Server creates. Pass `nil` if you require a function result but no authorization reference.

## Return Value

A result code. See Authorization Services Result Codes.

## Discussion

The primary purpose of this function is to create the opaque authorization reference structure associated with the authorization reference. You use the authorization reference in other authorization functions.

You can use this function to authorize all or partial rights. Authorizing rights with this function is most useful for applications that require a one-time authorization. By passing `nil` to the `authorization` parameter, the Security Server attempts to authorize the requested rights and returns the appropriate result code without actually granting the rights. If you are not going to call any other authorization functions, use this method to determine if a user has authorization without granting any rights.

You can also use this function to preauthorize rights by specifying the preAuthorize mask. Preauthorization is most useful when a right has a zero timeout. For example, you can preauthorize in the application and if it succeeds, call the helper tool and request authorization. This eliminates calling the helper tool if the user cannot later authorize the specified rights.

If you do not specify the partialRights mask and the Security Server denies at least one right, then the status of this function on return is errAuthorizationDenied.

If you do not specify the interactionAllowed mask and the Security Server requires user interaction, then the status of this function on return is errAuthorizationInteractionNotAllowed.

If you specify the interactionAllowed mask and the user cancels the authentication process, then the status of this function on return is errAuthorizationCanceled.

When your application no longer needs the authorization reference, use the function AuthorizationFree(_:_:) to free the memory associated with it.

