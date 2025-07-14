

- Quick Look
- QLGeneratorInterfaceStruct
-  Release 

Instance Property

# Release

macOS 10.5+

``` source
var Release: ((UnsafeMutableRawPointer?) -> ULONG)!
```

## See Also

### Creating a Quick Look Plug-In

init()

Creates the interface structure that the platform uses to interface with a Quick Look plug-in.

var QueryInterface: ((UnsafeMutableRawPointer?, REFIID, UnsafeMutablePointer&lt;LPVOID?>?) -> HRESULT)!

var AddRef: ((UnsafeMutableRawPointer?) -> ULONG)!

var GenerateThumbnailForURL: ((UnsafeMutableRawPointer?, QLThumbnailRequest?, CFURL?, CFString?, CFDictionary?, CGSize) -> OSStatus)!

var CancelThumbnailGeneration: ((UnsafeMutableRawPointer?, QLThumbnailRequest?) -> Void)!

var GeneratePreviewForURL: ((UnsafeMutableRawPointer?, QLPreviewRequest?, CFURL?, CFString?, CFDictionary?) -> OSStatus)!

var CancelPreviewGeneration: ((UnsafeMutableRawPointer?, QLPreviewRequest?) -> Void)!

