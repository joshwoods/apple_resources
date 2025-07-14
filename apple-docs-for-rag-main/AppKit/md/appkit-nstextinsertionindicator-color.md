

- AppKit
- NSTextInsertionIndicator
-  color 

Instance Property

# color

The color of this indicator.

macOS 14.0+

``` source
@NSCopying @MainActor
var color: NSColor! { get set }
```

## Discussion

If set to Nil, returns textInsertionPointColor. Defaults to textInsertionPointColor.

## See Also

### Configuring indicators

var effectsViewInserter: ((NSView) -> Void)?

An optional closure the system calls during dictation.

