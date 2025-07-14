

- AppKit
- NSTextLayoutManager
-  usesFontLeading 

Instance Property

# usesFontLeading

A Boolean value that controls whether the framework uses the leading information specified by the font when laying out text.

macOS 12.0+

``` source
var usesFontLeading: Bool { get set }
```

## Discussion

If set to `true`, uses the leading as specified by the font. However, this isn’t appropriate for most UI text. Defaults to `true`.

## See Also

### Configuring global layout manager options

var layoutQueue: OperationQueue?

The queue that the framework dispatches layout operations on.

var renderingAttributesValidator: ((NSTextLayoutManager, NSTextLayoutFragment) -> Void)?

A callback block that the framework invokes whenever the text layout manager needs to validate the rendering attributes for the range.

var usesHyphenation: Bool

A Boolean values that controls whether the text layout manager attempts to hyphenate when wrapping lines.

var limitsLayoutForSuspiciousContents: Bool

A Boolean value that controls internal security analysis for malicious inputs and activates defensive behaviors.

