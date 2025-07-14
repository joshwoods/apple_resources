

- Core Services
- Launch Services
-  LSRolesMask 

Structure

# LSRolesMask

The specification that sets the desired role or roles for an app to claim for an item or a family of items.

Mac Catalyst 13.0+macOS 10.0+

``` source
struct LSRolesMask
```

## Overview

This bit mask is passed to functions that find the preferred app for an item or family of items (`LSGetApplicationForItem`, `LSGetApplicationForURL`, `LSGetApplicationForInfo`), or that determine whether an app can open a designated item (`LSCanRefAcceptItem`, `LSCanURLAcceptURL`), to specify the app’s desired role or roles for the item. For example, to request only an editor app, specify `kLSRolesEditor`. If either an editor or a viewer app is acceptable, specify `kLSRolesEditor | kLSRolesViewer`.

## Topics

### Constants

static var none: LSRolesMask

Requests the role `None` (theapplication cannot open the item, but provides an icon and a kindstring for it).

static var viewer: LSRolesMask

Requests the role `Viewer` (theapplication can read and present the item, but cannot manipulateor save it).

static var editor: LSRolesMask

Requests the role `Editor` (theapplication can read, present, manipulate, and save the item).

static var shell: LSRolesMask

Requests the role `Shell` (theapplication can execute the item).

static var all: LSRolesMask

Accepts any role with respect to the item.

### Creating a Roles Mask

init(rawValue: OptionBits)

## Relationships

### Conforms To

- OptionSet
- Sendable

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

func LSSetDefaultHandlerForURLScheme(CFString, CFString) -> OSStatus

Sets the user’s preferred default handler for the specified URL scheme.

Deprecated

