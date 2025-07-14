

- Security
-  AuthorizationCopyRights(\_:\_:\_:\_:\_:) 

Function

# AuthorizationCopyRights(\_:\_:\_:\_:\_:)

Authorizes and preauthorizes rights synchronously.

Mac Catalyst 13.0+macOS 10.0+

``` source
func AuthorizationCopyRights(
    _ authorization: AuthorizationRef,
    _ rights: UnsafePointer,
    _ environment: UnsafePointer?,
    _ flags: AuthorizationFlags,
    _ authorizedRights: UnsafeMutablePointer?>?
) -> OSStatus
```

## Parameters 

`authorization`  

An authorization reference referring to the authorization session.

`rights`  

A pointer to a set of authorization rights you create. Pass `nil` if the application requires no rights at this time.

`environment`  

Data used when authorizing or preauthorizing rights. Not used in OS X v10.2 and earlier. In macOS 10.3 and later, you can pass icon or prompt data to be used in the authentication dialog box. In macOS 10.4 and later, you can also pass a user name and password in order to authorize a user without displaying the authentication dialog box. Possible values for this parameter are listed in `Security.framework/Headers/AuthorizationTags.h`. The data passed in this parameter is not stored in the authorization reference; it is used only during authorization. If you are not passing any data in this parameter, pass the constant kAuthorizationEmptyEnvironment.

`flags`  

A bit mask for specifying authorization options. Use the following option sets.

- Pass the constant kAuthorizationFlagDefaults if no options are necessary.

- Specify the extendRights mask to request rights. You can also specify the interactionAllowed mask to allow user interaction.

- Specify the partialRights and extendRights masks to request partial rights. You can also specify the interactionAllowed mask to allow user interaction.

- Specify the preAuthorize and extendRights masks to preauthorize rights.

- Specify the destroyRights mask to prevent the Security Server from preserving the rights obtained during this call.

`authorizedRights`  

A pointer to a newly allocated AuthorizationRights structure. On return, this structure contains the rights granted by the Security framework. If you do not require this information, pass `nil`. If you specify the preAuthorize mask in the `flags` parameter, the method returns all the requested rights, including those not granted, but the flags of the rights that could not be preauthorized include the kAuthorizationFlagCanNotPreAuthorize bit. Free the memory associated with this set by calling the function AuthorizationFreeItemSet(_:).

## Return Value

A result code. See Authorization Services Result Codes.

## Mentioned in 

Extending authorization services with plug-ins

## Discussion

There are three main reasons to use this function. The first reason is to preauthorize rights by specifying the preAuthorize, interactionAllowed, and extendRights masks as authorization options. Preauthorization is most useful when a right has a zero timeout. For example, you can preauthorize in the application and if it succeeds, call the helper tool and request authorization. This eliminates calling the helper tool if the Security Server cannot later authorize the specified rights.

The second reason to use this function is to authorize rights before performing a privileged operation by specifying the interactionAllowed, and extendRights masks as authorization options.

The third reason to use this function is to authorize partial rights. By specifying the partialRights, interactionAllowed, and extendRights masks as authorization options, the Security Server grants all rights it can authorize. On return, the authorized set contains all the rights.

If you do not specify the partialRights mask and the Security Server denies at least one right, then the status of this function on return is errAuthorizationDenied.

If you do not specify the interactionAllowed mask and the Security Server requires user interaction, then the status of this function on return is errAuthorizationInteractionNotAllowed.

If you specify the interactionAllowed mask and the user cancels the authentication process, then the status of this function on return is errAuthorizationCanceled.

