

- Core Services
- Launch Services
- Deprecated Symbols
-  kLSItemFileType Deprecated

Global Variable

# kLSItemFileType

The item’s file type.

Mac Catalyst 13.1–13.1DeprecatedmacOS 10.4–10.10Deprecated

``` source
let kLSItemFileType: CFString!
```

## Discussion

Use the URL resource property kCFURLTypeIdentifierKey/typeIdentifierKey to get the file's UTI instead.

## See Also

### Deprecated Constants

let kLSItemContentType: CFString!

The item’s content type identifier, which is a uniform type identifier string.

Deprecated

let kLSItemFileCreator: CFString!

The item’s file creator.

Deprecated

let kLSItemExtension: CFString!

The item’s filename extension.

Deprecated

let kLSItemDisplayName: CFString!

The item’s name to display to the user. The display name reflects localization and extension hiding that may be in effect.

Deprecated

let kLSItemDisplayKind: CFString!

The localized kind string that describes the item’s type.

Deprecated

let kLSItemRoleHandlerDisplayName: CFString!

The display name of the application that is set to handle this item, subject to the role mask.

Deprecated

let kLSItemIsInvisible: CFString!

A Boolean value that indicates the item is hidden from users.

Deprecated

let kLSItemExtensionIsHidden: CFString!

A Boolean value that indicates the item’s extension is hidden.

Deprecated

