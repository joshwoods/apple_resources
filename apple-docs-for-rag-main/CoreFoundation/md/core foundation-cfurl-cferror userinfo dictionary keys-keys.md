

- Core Foundation
- CFURL
-  CFError userInfo Dictionary Keys 

API Collection

# CFError userInfo Dictionary Keys

Keys in the userInfo dictionary of a `CFError` object when certain CFURL functions return an error.

## Topics

### Constants

let kCFURLKeysOfUnsetValuesKey: CFString!

Key for the resource properties that have not been set after the CFURLSetResourcePropertiesForKeys(_:_:_:) function returns an error, returned as an array of `CFString` objects.

## See Also

### File System Constants

Common File System Resource Keys

Keys that are applicable to file system URLs.

File Resource Types

Possible values for the kCFURLFileResourceTypeKey key.

File Property Keys

Keys that apply to properties of files.

iCloud Constants

These constants can be used to determining whether a file is stored in the cloud and to obtain information about its status.

Volume Property Keys

Keys that apply to volumes.

