

- Core Services
- Launch Services
-  LSCopyAllRoleHandlersForContentType(\_:\_:) Deprecated

Function

# LSCopyAllRoleHandlersForContentType(\_:\_:)

Locates an array of bundle identifiers for apps capable of handling a specified content type with the specified roles.

macOS 10.4–12.0Deprecated

``` source
func LSCopyAllRoleHandlersForContentType(
    _ inContentType: CFString,
    _ inRole: LSRolesMask
) -> Unmanaged?
```

## Parameters 

`inContentType`  

The content type. The content type is a uniform type identifier.

`inRole`  

The role. Pass `kLSRolesAll` if any role is acceptable. For additional possible values, see LSRolesMask.

## Return Value

The bundle identifiers for apps capable of handling the specified content type in the specified roles, or `NULL` if no handlers are available.

In macOS 10.15 and later, the returned array is sorted so that the first element contains the bundle identifier of the best available app for opening the content type. Prior to macOS 10.15, the order of elements in the array was undefined.

## Discussion

This function returns all of the bundle identifiers that are capable of handling the specified content type in the specified roles.

The CFBundleDocumentTypes key in an app’s `Info.plist` can be used to set an app’s content handling capabilities. The LSItemContentTypes key is particularly useful because it supports the use of UTIs in document claims.

### Version Notes

Thread-safe since macOS 10.4.

## See Also

### Working with Role Handlers

func LSCopyDefaultRoleHandlerForContentType(CFString, LSRolesMask) -> Unmanaged&lt;CFString>?

Returns the bundle identifier of the user’s preferred default handler for the specified content type with the specified role.

Deprecated

func LSSetDefaultRoleHandlerForContentType(CFString, LSRolesMask, CFString) -> OSStatus

Sets the user’s preferred default handler for the specified content type in the specified roles.

Deprecated

func LSSetDefaultHandlerForURLScheme(CFString, CFString) -> OSStatus

Sets the user’s preferred default handler for the specified URL scheme.

Deprecated

struct LSRolesMask

The specification that sets the desired role or roles for an app to claim for an item or a family of items.

