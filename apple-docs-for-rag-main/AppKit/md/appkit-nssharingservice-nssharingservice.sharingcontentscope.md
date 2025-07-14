

- AppKit
- NSSharingService
-  NSSharingService.SharingContentScope 

Enumeration

# NSSharingService.SharingContentScope

The sharing scope constants specify the nature of the things you are sharing.

macOS 10.8+

``` source
enum SharingContentScope
```

## Topics

### Constants

case item

Used when sharing a clearly identified item, for example, a file represented by its icon.

case partial

Used when sharing a portion of a more global content, for example, part of a webpage.

case full

Used when sharing the whole content of the current document, for example, the URL of the webpage.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Customizing Transition Animation

func sharingService(NSSharingService, sourceFrameOnScreenForShareItem: Any) -> NSRect

Invoked when the sharing service is performed and the sharing window is displayed, to present a transition between the original items and the sharing window.

func sharingService(NSSharingService, transitionImageForShareItem: Any, contentRect: UnsafeMutablePointer&lt;NSRect>) -> NSImage?

Invoked to allow returning a custom transition image when sharing an item.

func sharingService(NSSharingService, sourceWindowForShareItems: [Any], sharingContentScope: UnsafeMutablePointer&lt;NSSharingService.SharingContentScope>) -> NSWindow?

Returns the window that contained the share items.

