

- AppKit
- NSPathControl
-  backgroundColor 

Instance Property

# backgroundColor

The receiver’s background color.

macOS 10.5+

``` source
@NSCopying @MainActor
var backgroundColor: NSColor? { get set }
```

## Discussion

By default, the background is set to a light blue color for `NSPathStyleStandard` and `nil` for the other styles. You can use `[NSColor clearColor]` to make the background transparent.

