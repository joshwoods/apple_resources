

- Core Services
- Launch Services
-  LSCopyDefaultRoleHandlerForContentType(\_:\_:) Deprecated

Function

# LSCopyDefaultRoleHandlerForContentType(\_:\_:)

Returns the bundle identifier of the user’s preferred default handler for the specified content type with the specified role.

Mac Catalyst 13.1–15.0DeprecatedmacOS 10.4–12.0Deprecated

``` source
func LSCopyDefaultRoleHandlerForContentType(
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

The bundle identifier of the default handler for the specified content type in the specified roles, or `NULL` if no handler is available.

## Discussion

This function returns the user’s currently preferred default handler for the specified content type. Say, for example, that LSSetDefaultRoleHandlerForContentType(_:_:_:) has been used to set “com.Apple.TextEdit” for the “public.xml” content type. When a file whose content type is “public.xml” is double-clicked, TextEdit will be launched to open the file. If you call `LSCopyDefaultRoleHandlerForContentType(CFSTR(“public.xml”), kLSRolesAll)`, the string `com.apple.TextEdit` is returned.

The CFBundleDocumentTypes key in an app’s `Info.plist` can be used to set an app’s content handling capabilities. The `LSItemContentTypes` key is particularly useful because it supports the use of UTIs in document claims.

### Version-Notes

Thread-safe since OS X v10.4.

## See Also

### Working with Role Handlers

func LSCopyAllRoleHandlersForContentType(CFString, LSRolesMask) -> Unmanaged&lt;CFArray>?

Locates an array of bundle identifiers for apps capable of handling a specified content type with the specified roles.

Deprecated

func LSSetDefaultRoleHandlerForContentType(CFString, LSRolesMask, CFString) -> OSStatus

Sets the user’s preferred default handler for the specified content type in the specified roles.

Deprecated

func LSSetDefaultHandlerForURLScheme(CFString, CFString) -> OSStatus

Sets the user’s preferred default handler for the specified URL scheme.

Deprecated

struct LSRolesMask

The specification that sets the desired role or roles for an app to claim for an item or a family of items.

