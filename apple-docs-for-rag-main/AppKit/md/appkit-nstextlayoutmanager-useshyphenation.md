

- AppKit
- NSTextLayoutManager
-  usesHyphenation 

Instance Property

# usesHyphenation

A Boolean values that controls whether the text layout manager attempts to hyphenate when wrapping lines.

macOS 12.0+

``` source
var usesHyphenation: Bool { get set }
```

## Discussion

Defaults to `true`.

## See Also

### Configuring global layout manager options

var layoutQueue: OperationQueue?

The queue that the framework dispatches layout operations on.

var renderingAttributesValidator: ((NSTextLayoutManager, NSTextLayoutFragment) -> Void)?

A callback block that the framework invokes whenever the text layout manager needs to validate the rendering attributes for the range.

var usesFontLeading: Bool

A Boolean value that controls whether the framework uses the leading information specified by the font when laying out text.

var limitsLayoutForSuspiciousContents: Bool

A Boolean value that controls internal security analysis for malicious inputs and activates defensive behaviors.

