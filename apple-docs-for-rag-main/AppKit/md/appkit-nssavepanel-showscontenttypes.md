

- AppKit
- NSSavePanel
-  showsContentTypes 

Instance Property

# showsContentTypes

`NSSavePanel`: Whether or not to show a control for selecting the type of the saved file. The control shows the types in `allowedContentTypes`. Default is `NO`.

macOS 15.0+

``` source
@MainActor
var showsContentTypes: Bool { get set }
```

## Discussion

Note

If @c allowedContentTypes is empty, the control is not displayed. `NSOpenPanel`: Not used.

