

- Core Services
- Launch Services
-  LSSharedFileListItem 

Class

# LSSharedFileListItem

A file-system object in the shared file list.

Mac Catalyst 16.0+macOS 10.5+

``` source
class LSSharedFileListItem
```

## See Also

### Opening Items

func LSOpenCFURLRef(CFURL, UnsafeMutablePointer&lt;Unmanaged&lt;CFURL>?>?) -> OSStatus

Opens an item for a URL in the default manner in its preferred app.

func LSOpenFromURLSpec(UnsafePointer&lt;LSLaunchURLSpec>, UnsafeMutablePointer&lt;Unmanaged&lt;CFURL>?>?) -> OSStatus

Opens one or more items for a URL in the preferred apps or a designated app.

struct LSLaunchURLSpec

The specification for launching an app, opening items, or both, along with related information.

class LSSharedFileList

A persistent list of file-system objects.

