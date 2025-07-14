

- AppKit
- NSSavePanel
-  currentContentType 

Instance Property

# currentContentType

`NSSavePanel`:The current type. If set to `nil`, resets to the first allowed content type. Returns `nil` if `allowedContentTypes` is empty. `NSOpenPanel`: Not used.

macOS 15.0+

``` source
@MainActor
var currentContentType: UTType? { get set }
```

## Discussion

Note

Asserts that `currentContentType` conforms to `UTTypeData` or `UTTypeDirectory`.

