

- Application Services
- ApplicationServices Structures
- ICMapEntry
-  init(totalLength:fixedLength:version:fileType:fileCreator:postCreator:flags:extension:creatorAppName:postAppName:MIMEType:entryName:) 

Initializer

# init(totalLength:fixedLength:version:fileType:fileCreator:postCreator:flags:extension:creatorAppName:postAppName:MIMEType:entryName:)

macOS 10.9+Xcode 9.0+

``` source
init(
    totalLength: Int16,
    fixedLength: ICFixedLength,
    version: Int16,
    fileType: OSType,
    fileCreator: OSType,
    postCreator: OSType,
    flags: ICMapEntryFlags,
    extension: Str255,
    creatorAppName: Str255,
    postAppName: Str255,
    MIMEType: Str255,
    entryName: Str255
)
```

