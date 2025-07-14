

- Application Services
- ApplicationServices Structures
-  ICMapEntry 

Structure

# ICMapEntry

macOS 10.0+

``` source
struct ICMapEntry
```

## Topics

### Initializers

init()

init(totalLength: Int16, fixedLength: ICFixedLength, version: Int16, fileType: OSType, fileCreator: OSType, postCreator: OSType, flags: ICMapEntryFlags, extension: Str255, creatorAppName: Str255, postAppName: Str255, MIMEType: Str255, entryName: Str255)

### Instance Properties

var MIMEType: Str255

var creatorAppName: Str255

var entryName: Str255

var `extension`: Str255

var fileCreator: OSType

var fileType: OSType

var fixedLength: ICFixedLength

var flags: ICMapEntryFlags

var postAppName: Str255

var postCreator: OSType

var totalLength: Int16

var version: Int16

