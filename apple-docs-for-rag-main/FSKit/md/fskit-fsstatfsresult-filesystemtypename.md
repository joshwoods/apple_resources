

- FSKit
- FSStatFSResult
-  fileSystemTypeName 

Instance Property

# fileSystemTypeName

A property for the file system type name.

macOS 15.4+

``` source
var fileSystemTypeName: String { get }
```

## Discussion

Match this value to the `FSShortName` attribute within the `EXAppExtensionAttributes` dictionary of the module’s `Info.plist`. The maximum allowed length is `MFSTYPENAMELEN`, including the terminating `NUL` character.

