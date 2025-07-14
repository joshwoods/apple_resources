

- AppKit
- NSMediaLibraryBrowserController
-  NSMediaLibraryBrowserController.Library 

Structure

# NSMediaLibraryBrowserController.Library

These constants are masks used to configure a Media Library Browser to display specific types of media. Combined masks are not yet supported. In other words, only one nonzero mask value is supported at a time. If masks are combined, the lowest mask value is used.

macOS 10.9+

``` source
struct Library
```

## Topics

### Constants

static var audio: NSMediaLibraryBrowserController.Library

Display audio media.

static var image: NSMediaLibraryBrowserController.Library

Display image media.

static var movie: NSMediaLibraryBrowserController.Library

Display movie media.

### Initializers

init(rawValue: UInt)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- ExpressibleByArrayLiteral
- OptionSet
- RawRepresentable
- Sendable
- SetAlgebra

