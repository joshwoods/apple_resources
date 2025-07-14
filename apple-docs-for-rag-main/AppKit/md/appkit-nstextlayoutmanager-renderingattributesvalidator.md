

- AppKit
- NSTextLayoutManager
-  renderingAttributesValidator 

Instance Property

# renderingAttributesValidator

A callback block that the framework invokes whenever the text layout manager needs to validate the rendering attributes for the range.

macOS 12.0+

``` source
var renderingAttributesValidator: ((NSTextLayoutManager, NSTextLayoutFragment) -> Void)? { get set }
```

## Discussion

The validator uses setRenderingAttributes(_:for:) to fill the rendering attributes appropriate for the range inside `textLayoutFragment`.

## See Also

### Configuring global layout manager options

var layoutQueue: OperationQueue?

The queue that the framework dispatches layout operations on.

var usesFontLeading: Bool

A Boolean value that controls whether the framework uses the leading information specified by the font when laying out text.

var usesHyphenation: Bool

A Boolean values that controls whether the text layout manager attempts to hyphenate when wrapping lines.

var limitsLayoutForSuspiciousContents: Bool

A Boolean value that controls internal security analysis for malicious inputs and activates defensive behaviors.

