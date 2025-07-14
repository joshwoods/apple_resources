

- AppKit
- NSSavePanel
-  url 

Instance Property

# url

A URL that contains the fully specified location of the targeted file.

macOS

``` source
@MainActor
var url: URL? { get }
```

## Discussion

The NSOpenPanel subclass sets this property to `nil` when the selection contains multiple items.

