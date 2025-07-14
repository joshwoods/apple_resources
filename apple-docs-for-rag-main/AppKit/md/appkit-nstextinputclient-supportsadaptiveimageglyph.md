

- AppKit
- NSTextInputClient
-  supportsAdaptiveImageGlyph 

Instance Property

# supportsAdaptiveImageGlyph

A Boolean value that indicates whether the document supports adaptive images in the input.

macOS 15.0+

``` source
optional var supportsAdaptiveImageGlyph: Bool { get }
```

## Discussion

When this property is false, the input system doesn’t allow the text input to contain adaptive images. Set the value of this property to true only if your document supports adaptive images and handles them properly. For more information, see NSAdaptiveImageGlyph.

## See Also

### Supporting adaptive images

func insert(NSAdaptiveImageGlyph, replacementRange: NSRange)

Inserts an adaptive image into the text at the specifed location.

