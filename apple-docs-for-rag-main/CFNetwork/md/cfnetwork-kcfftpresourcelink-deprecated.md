

- CFNetwork
-  kCFFTPResourceLink Deprecated

Global Variable

# kCFFTPResourceLink

CFDictionary key for getting the CFString containing the symbolic link information. If the item is a symbolic link, the CFString contains the path to the item that the link references.

iOS 2.0–9.0DeprecatediPadOS 2.0–9.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.3–10.11DeprecatedtvOS 9.0–9.0DeprecatedvisionOS 1.0–1.0Deprecated

``` source
let kCFFTPResourceLink: CFString
```

Deprecated

Use NSURLSessionAPI for ftp requests

## See Also

### FTP

func CFFTPCreateParsedResourceListing(CFAllocator?, UnsafePointer&lt;UInt8>, CFIndex, UnsafeMutablePointer&lt;Unmanaged&lt;CFDictionary>?>?) -> CFIndex

Parses an FTP listing to a dictionary.

Deprecated

let kCFFTPResourceGroup: CFString

CFDictionary key for getting the CFString containing the name of a group that shares the FTP resource.

Deprecated

let kCFFTPResourceModDate: CFString

CFDictionary key for getting the CFDate containing the last date and time the FTP resource was modified.

Deprecated

let kCFFTPResourceMode: CFString

CFDictionary key for getting the CFNumber containing the access permissions, defined in `sys/types.h`, of the FTP resource.

Deprecated

let kCFFTPResourceName: CFString

CFDictionary key for getting the CFString containing the name of the FTP resource.

Deprecated

let kCFFTPResourceOwner: CFString

CFDictionary key for getting the CFString containing the name of the owner of the FTP resource.

Deprecated

let kCFFTPResourceSize: CFString

CFDictionary key for getting the CFNumber containing the size in bytes of the FTP resource.

Deprecated

let kCFFTPResourceType: CFString

CFDictionary key for getting the CFNumber containing the type of the FTP resource as defined in `sys/dirent.h`.

Deprecated

