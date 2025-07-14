

- Core Foundation
- CFURL
-  iCloud Constants 

API Collection

# iCloud Constants

These constants can be used to determining whether a file is stored in the cloud and to obtain information about its status.

## Topics

### Constants

let kCFURLIsUbiquitousItemKey: CFString!

A `CFBoolean` value that tells whether the item is synced to the cloud. (read-only)

let kCFURLUbiquitousItemHasUnresolvedConflictsKey: CFString!

A `CFBoolean` value that tells whether the item has conflicts outstanding. (read-only)

let kCFURLUbiquitousItemIsDownloadedKey: CFString!

A `CFBoolean` value that tells whether there is local data present for the item. (read-only)

Deprecated

let kCFURLUbiquitousItemIsDownloadingKey: CFString!

A `CFBoolean` value that tells whether data for the item is being downloaded. (read-only)

let kCFURLUbiquitousItemIsUploadedKey: CFString!

A `CFBoolean` value that tells whether there is data present in the cloud for this item. (read-only)

let kCFURLUbiquitousItemIsUploadingKey: CFString!

A `CFBoolean` value that tells whether data for the item is being uploaded. (read-only)

let kCFURLUbiquitousItemPercentDownloadedKey: CFString!Deprecated

let kCFURLUbiquitousItemPercentUploadedKey: CFString!Deprecated

## See Also

### File System Constants

Common File System Resource Keys

Keys that are applicable to file system URLs.

File Resource Types

Possible values for the kCFURLFileResourceTypeKey key.

File Property Keys

Keys that apply to properties of files.

Volume Property Keys

Keys that apply to volumes.

CFError userInfo Dictionary Keys

Keys in the userInfo dictionary of a `CFError` object when certain CFURL functions return an error.

