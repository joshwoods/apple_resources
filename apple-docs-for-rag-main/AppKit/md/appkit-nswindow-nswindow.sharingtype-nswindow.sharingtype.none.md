

- AppKit
- NSWindow
- NSWindow.SharingType
-  NSWindow.SharingType.none 

Case

# NSWindow.SharingType.none

A legacy constant that macOS no longer uses.

macOS 10.5+

``` source
case none
```

## Discussion

`NSWindowSharingNone` can cause content to not be available in certain sharing situations. Don’t use this value to hide or omit content from being captured. Instead, use FairPlay Streaming (FPS). For more information, read FairPlay Streaming.

## See Also

### Constants

case readOnly

static let readWrite: NSWindow.SharingTypeDeprecated

