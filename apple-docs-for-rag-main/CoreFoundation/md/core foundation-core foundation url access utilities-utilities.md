

- Core Foundation
-  Core Foundation URL Access Utilities 

API Collection

# Core Foundation URL Access Utilities

## Overview

Core Foundation URL Access Utilities give you convenient system-independent methods of creating, reading, updating, or deleting a URL resource.

Given a CFURL object that holds either a file or http URL, you can read the resource’s data with the CFURLCreateDataAndPropertiesFromResource(_:_:_:_:_:_:) function. You can write data to the URL resource, possibly creating a new file, with the CFURLWriteDataAndPropertiesToResource(_:_:_:_:) function. Finally, you can destroy, or delete, the resource pointed to by the URL with the CFURLDestroyResource(_:_:) function.

## Topics

### Core Foundation URL Access Utilities Miscellaneous Functions

func CFURLCreateDataAndPropertiesFromResource(CFAllocator!, CFURL!, UnsafeMutablePointer&lt;Unmanaged&lt;CFData>?>!, UnsafeMutablePointer&lt;Unmanaged&lt;CFDictionary>?>!, CFArray!, UnsafeMutablePointer&lt;Int32>!) -> Bool

Loads the data and properties referred to by a given URL.

Deprecated

func CFURLCreatePropertyFromResource(CFAllocator!, CFURL!, CFString!, UnsafeMutablePointer&lt;Int32>!) -> CFTypeRef!

Returns a given property specified by a given URL and property string.

Deprecated

func CFURLDestroyResource(CFURL!, UnsafeMutablePointer&lt;Int32>!) -> Bool

Destroys a resource indicated by a given URL.

Deprecated

func CFURLWriteDataAndPropertiesToResource(CFURL!, CFData!, CFDictionary!, UnsafeMutablePointer&lt;Int32>!) -> Bool

Writes the given data and properties to a given URL.

Deprecated

### Constants

enum CFURLError

`CFURL` error codes.

Deprecated

File URL Properties

Properties for file URL resources.

HTTP URL Properties

Properties for HTTP URL resources.

## See Also

### Utilities

Base Utilities

Byte-Order Utilities

Preferences Utilities

Socket Name Server Utilities

Time Utilities

