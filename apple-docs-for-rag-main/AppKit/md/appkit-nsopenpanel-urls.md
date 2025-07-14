

- AppKit
- NSOpenPanel
-  urls 

Instance Property

# urls

An array of URLs, each of which contains the fully specified location of a selected file or directory.

macOS

``` source
@MainActor
var urls: [URL] { get }
```

## Discussion

This property contains a valid value when the user selects one item or multiple items.

