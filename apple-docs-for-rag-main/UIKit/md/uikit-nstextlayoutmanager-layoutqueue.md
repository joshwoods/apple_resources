

- UIKit
- NSTextLayoutManager
-  layoutQueue 

Instance Property

# layoutQueue

The queue that the framework dispatches layout operations on.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+tvOS 15.0+visionOS 1.0+

``` source
var layoutQueue: OperationQueue? { get set }
```

## Discussion

If non-`nil`, it performs layout in the specified queue until `estimatedUsageBounds` becomes `false`.

## See Also

### Configuring global layout manager options

var renderingAttributesValidator: ((NSTextLayoutManager, NSTextLayoutFragment) -> Void)?

A callback block that the framework invokes whenever the text layout manager needs to validate the rendering attributes for the range.

var usesFontLeading: Bool

A Boolean value that controls whether the framework uses the leading information specified by the font when laying out text.

var usesHyphenation: Bool

A Boolean values that controls whether the text layout manager attempts to hyphenate when wrapping lines.

var limitsLayoutForSuspiciousContents: Bool

A Boolean value that controls internal security analysis for malicious inputs and activates defensive behaviors.

