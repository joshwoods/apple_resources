

- Core Services
- Launch Services
-  LSSetDefaultHandlerForURLScheme(\_:\_:) Deprecated

Function

# LSSetDefaultHandlerForURLScheme(\_:\_:)

Sets the user’s preferred default handler for the specified URL scheme.

Mac Catalyst 13.1–15.0DeprecatedmacOS 10.4–12.0Deprecated

``` source
func LSSetDefaultHandlerForURLScheme(
    _ inURLScheme: CFString,
    _ inHandlerBundleID: CFString
) -> OSStatus
```

## Parameters 

`inURLScheme`  

The URL scheme for which the handler is to be set.

`inHandlerBundleID`  

The bundle identifier that is to be set as the handler for the URL scheme specified by `inURLScheme`.

## Return Value

A result code; see Result Codes.

## Discussion

Call LSCopyDefaultHandlerForURLScheme(_:) to get the current setting of the user’s preferred default handler for a specified content type.

URL handling capability is determined according to the value of the `CFBundleURLTypes` key in an app’s `Info.plist`. For information on the `CFBundleURLTypes` key, see the section “CFBundleURLTypes” in *macOS Runtime Configuration Guidelines*.

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

func LSSetDefaultRoleHandlerForContentType(CFString, LSRolesMask, CFString) -> OSStatus

Sets the user’s preferred default handler for the specified content type in the specified roles.

Deprecated

struct LSRolesMask

The specification that sets the desired role or roles for an app to claim for an item or a family of items.

