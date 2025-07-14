

- UIKit
- UITextInput
-  supportsAdaptiveImageGlyph 

Instance Property

# supportsAdaptiveImageGlyph

A Boolean value that indicates whether the document supports adaptive images in the input.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+tvOS 18.0+visionOS 2.0+

``` source
@MainActor
optional var supportsAdaptiveImageGlyph: Bool { get set }
```

## Discussion

When this property is false, the input system doesn’t allow the text input to contain adaptive images. Set the value of this property to true only if your document supports adaptive images and handles them properly. For more information, see NSAdaptiveImageGlyph

## See Also

### Supporting adaptive images

func insert(NSAdaptiveImageGlyph, replacementRange: UITextRange)

Inserts an adaptive image into the text at the specifed location.

