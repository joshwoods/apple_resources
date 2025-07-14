

- Core Foundation
-  kCFURLFileOwnerID Deprecated

Global Variable

# kCFURLFileOwnerID

A `CFNumber` holding the file owner’s UID.

tvOS 9.0–9.0DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 2.0–2.0Deprecated

``` source
let kCFURLFileOwnerID: CFString!
```

Deprecated

Use CFURLCopyResourcePropertyForKey with kCFURLFileSecurityKey and then the CFFileSecurity API instead.

## See Also

### Constants

let kCFURLFileExists: CFString!

A `CFBoolean` object indicating whether the file referred to by a URL exists.

Deprecated

let kCFURLFileDirectoryContents: CFString!

A `CFArray` object holding `CFURL` objects for the contents of a directory referred to by a URL.

Deprecated

let kCFURLFileLength: CFString!

A `CFNumber` object holding the file’s length in bytes.

Deprecated

let kCFURLFileLastModificationTime: CFString!

A `CFDate` object holding the file’s modification time.

Deprecated

let kCFURLFilePOSIXMode: CFString!

A `CFNumber` holding the file’s POSIX mode as given in `/usr/include/sys/stat.h`.

Deprecated

