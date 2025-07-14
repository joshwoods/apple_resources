

- Core Foundation
- CFURL
-  File Property Keys 

API Collection

# File Property Keys

Keys that apply to properties of files.

## Topics

### Constants

let kCFURLFileAllocatedSizeKey: CFString!

Key for the total size allocated on disk for the file, returned as an `CFNumber` object.

let kCFURLFileSizeKey: CFString!

Key for the file’s size in bytes, returned as a `CFNumber` object.

let kCFURLIsAliasFileKey: CFString!

Key for determining whether the file is an alias, returned as a `CFBoolean` object.

let kCFURLIsMountTriggerKey: CFString!

Key for determining whether the URL is a file system trigger directory, returned as a `CFBoolean` object. Traversing or opening a file system trigger directory causes an attempt to mount a file system on the directory.

let kCFURLTotalFileAllocatedSizeKey: CFString!

Key for the total allocated size of the file in bytes, returned as a `CFNumber` object. This includes the size of any file metadata.

let kCFURLTotalFileSizeKey: CFString!

Key for the total displayable size of the file in bytes, returned as a `CFNumber` object. This includes the size of any file metadata.

## See Also

### File System Constants

Common File System Resource Keys

Keys that are applicable to file system URLs.

File Resource Types

Possible values for the kCFURLFileResourceTypeKey key.

iCloud Constants

These constants can be used to determining whether a file is stored in the cloud and to obtain information about its status.

Volume Property Keys

Keys that apply to volumes.

CFError userInfo Dictionary Keys

Keys in the userInfo dictionary of a `CFError` object when certain CFURL functions return an error.

