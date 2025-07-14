

- Quick Look
- QLGeneratorInterfaceStruct
-  init() 

Initializer

# init()

Creates the interface structure that the platform uses to interface with a Quick Look plug-in.

macOS 10.5+

``` source
init()
```

## See Also

### Creating a Quick Look Plug-In

var QueryInterface: ((UnsafeMutableRawPointer?, REFIID, UnsafeMutablePointer&lt;LPVOID?>?) -> HRESULT)!

var AddRef: ((UnsafeMutableRawPointer?) -> ULONG)!

var Release: ((UnsafeMutableRawPointer?) -> ULONG)!

var GenerateThumbnailForURL: ((UnsafeMutableRawPointer?, QLThumbnailRequest?, CFURL?, CFString?, CFDictionary?, CGSize) -> OSStatus)!

var CancelThumbnailGeneration: ((UnsafeMutableRawPointer?, QLThumbnailRequest?) -> Void)!

var GeneratePreviewForURL: ((UnsafeMutableRawPointer?, QLPreviewRequest?, CFURL?, CFString?, CFDictionary?) -> OSStatus)!

var CancelPreviewGeneration: ((UnsafeMutableRawPointer?, QLPreviewRequest?) -> Void)!

