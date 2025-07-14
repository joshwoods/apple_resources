

- Core Services
- Launch Services
-  LSSetDefaultRoleHandlerForContentType(\_:\_:\_:) Deprecated

Function

# LSSetDefaultRoleHandlerForContentType(\_:\_:\_:)

Sets the user’s preferred default handler for the specified content type in the specified roles.

Mac Catalyst 13.1–15.0DeprecatedmacOS 10.4–12.0Deprecated

``` source
func LSSetDefaultRoleHandlerForContentType(
    _ inContentType: CFString,
    _ inRole: LSRolesMask,
    _ inHandlerBundleID: CFString
) -> OSStatus
```

## Parameters 

`inContentType`  

The content type for which the default role handler is being set. The content type is a uniform type identifier.

`inRole`  

The roles for which the default role handler is being set. Pass `kLSRolesAll` to specify all roles. For additional possible values, see LSRolesMask.

`inHandlerBundleID`  

The bundle identifier that is to be set as the default handler for the specified content type and roles.

## Return Value

A result code; see Result Codes.

## Discussion

Call LSCopyDefaultRoleHandlerForContentType(_:_:) to get the current setting of the user’s preferred default handler for a specified content type.

### Version-Notes

Thread-safe since OS X v10.4.

## See Also

### Working with Role Handlers

func LSCopyAllRoleHandlersForContentType(CFString, LSRolesMask) -> Unmanaged&lt;CFArray>?

Locates an array of bundle identifiers for apps capable of handling a specified content type with the specified roles.

Deprecated

func LSCopyDefaultRoleHandlerForContentType(CFString, LSRolesMask) -> Unmanaged&lt;CFString>?

Returns the bundle identifier of the user’s preferred default handler for the specified content type with the specified role.

Deprecated

func LSSetDefaultHandlerForURLScheme(CFString, CFString) -> OSStatus

Sets the user’s preferred default handler for the specified URL scheme.

Deprecated

struct LSRolesMask

The specification that sets the desired role or roles for an app to claim for an item or a family of items.

