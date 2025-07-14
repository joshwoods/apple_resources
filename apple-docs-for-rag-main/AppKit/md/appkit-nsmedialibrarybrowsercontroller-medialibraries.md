

- AppKit
- NSMediaLibraryBrowserController
-  mediaLibraries 

Instance Property

# mediaLibraries

The media library that is in use.

macOS 10.9+

``` source
var mediaLibraries: NSMediaLibraryBrowserController.Library { get set }
```

## Discussion

This property will be one of the values in the NSMediaLibraryBrowserController.Library constants.

You can set the value to use a specific library (image, audio or movie). You can also read the value to determine which is currently displayed.

