

- FSKit
- FSStatFSResult
-  fileSystemSubType 

Instance Property

# fileSystemSubType

A property for the file system’s subtype or flavor.

macOS 15.4+

``` source
var fileSystemSubType: Int { get set }
```

## Discussion

Match this value to the `FSPersonalities`‘s `FSSubType` attribute, if it exists within the `EXAppExtensionAttributes` dictionary of the module’s `Info.plist`.

