

- Core Foundation
-  kCFURLTotalFileAllocatedSizeKey 

Global Variable

# kCFURLTotalFileAllocatedSizeKey

Key for the total allocated size of the file in bytes, returned as a `CFNumber` object. This includes the size of any file metadata.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
let kCFURLTotalFileAllocatedSizeKey: CFString!
```

## See Also

### Constants

let kCFURLFileAllocatedSizeKey: CFString!

Key for the total size allocated on disk for the file, returned as an `CFNumber` object.

let kCFURLFileSizeKey: CFString!

Key for the file’s size in bytes, returned as a `CFNumber` object.

let kCFURLIsAliasFileKey: CFString!

Key for determining whether the file is an alias, returned as a `CFBoolean` object.

let kCFURLIsMountTriggerKey: CFString!

Key for determining whether the URL is a file system trigger directory, returned as a `CFBoolean` object. Traversing or opening a file system trigger directory causes an attempt to mount a file system on the directory.

let kCFURLTotalFileSizeKey: CFString!

Key for the total displayable size of the file in bytes, returned as a `CFNumber` object. This includes the size of any file metadata.

