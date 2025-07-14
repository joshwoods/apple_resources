

- Core Foundation
-  kCFURLCustomIconKey Deprecated

Global Variable

# kCFURLCustomIconKey

Key for the icon stored with the resource, returned as a `CGImageRef` object, or `NULL` if the resource has no custom icon.

iOS 4.0–10.0DeprecatediPadOS 4.0–10.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.6–10.12DeprecatedtvOS 9.0–10.0DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 2.0–3.0Deprecated

``` source
let kCFURLCustomIconKey: CFString!
```

Deprecated

Use NSURLCustomIconKey

## See Also

### Constants

let kCFURLNameKey: CFString!

Key for the resource’s name in the file system, returned as a `CFString` object.

let kCFURLLocalizedNameKey: CFString!

Key for the resource’s localized or extension-hidden name, retuned as a `CFString` object.

let kCFURLPathKey: CFString!

A `CFString` value containing the URL’s path as a file system path. (read-only)

let kCFURLIsRegularFileKey: CFString!

Key for determining whether the resource is a regular file, as opposed to a directory or a symbolic link. Returned as a `CFBoolean` object.

let kCFURLIsDirectoryKey: CFString!

Key for determining whether the resource is a directory, returned as a `CFBoolean` object.

let kCFURLIsSymbolicLinkKey: CFString!

Key for determining whether the resource is a symbolic link, returned as a `CFBoolean` object.

let kCFURLIsVolumeKey: CFString!

Key for determining whether the resource is the root directory of a volume, returned as a `CFBoolean` object.

let kCFURLIsPackageKey: CFString!

Key for determining whether the resource is a packaged directory, returned as a `CFBoolean` object.

let kCFURLIsSystemImmutableKey: CFString!

Key for determining whether the resource’s system immutable bit is set, returned as a `CFBoolean` object.

let kCFURLIsUserImmutableKey: CFString!

Key for determining whether the resource’s user immutable bit is set, returned as a `CFBoolean` object.

let kCFURLIsHiddenKey: CFString!

Key for determining whether the resource is normally not displayed to users, returned as a `CFBoolean` object.

let kCFURLHasHiddenExtensionKey: CFString!

Key for determining whether the resource’s extension is normally removed from its localized name, returned as a `CFBoolean` object.

let kCFURLCreationDateKey: CFString!

Key for the resource’s creation date, returned as a `CFDate` object if the volume supports creation dates, or `nil` if creation dates are unsupported.

let kCFURLContentAccessDateKey: CFString!

Key for the last time the resource was accessed, returned as a `CFDate` object if the volume supports access dates, or `nil` if access dates are unsupported.

let kCFURLContentModificationDateKey: CFString!

Key for the last time the resource was modified, returned as a `CFDate` object if the volume supports modification dates, or `nil` if modification dates are unsupported.

