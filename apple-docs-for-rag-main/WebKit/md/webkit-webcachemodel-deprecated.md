

- WebKit
-  WebCacheModel Deprecated

Enumeration

# WebCacheModel

Specifies the caching model for a web view.

macOS 10.5–10.14Deprecated

``` source
enum WebCacheModel
```

## Topics

### Constants

case documentViewer

Releases resources when they are no longer referenced and caches remote resources on disk. This model is appropriate for displaying a static document with no navigation user interface. This is the most memory-efficient model.

case documentBrowser

Caches a reasonable number of resources and previously viewed documents in memory and on disk. This model is appropriate for displaying and navigating between multiple documents.

case primaryWebBrowser

Caches a large number of resources and previously viewed documents in memory and on disk. This model is appropriate for a web view that behaves like a web browser.

### Initializers

init?(rawValue: UInt)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

