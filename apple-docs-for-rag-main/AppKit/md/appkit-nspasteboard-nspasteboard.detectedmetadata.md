

- AppKit
- NSPasteboard
-  NSPasteboard.DetectedMetadata 

Structure

# NSPasteboard.DetectedMetadata

An object that contains common types of metadata that the data detection system matches for a pasteboard.

macOS 15.4+

``` source
struct DetectedMetadata
```

## Topics

### Instance Properties

var contentType: UTType?

The content type that the data detection system identifies for a reference to a file that is present on the pasteboard.

var metadataTypes: Set&lt;PartialKeyPath&lt;NSPasteboard.DetectedMetadata>>

A set of key paths that represent metadata types that the data detection system identifies.

