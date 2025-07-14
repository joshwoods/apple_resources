

- AppKit
- NSTextInputClient
-  insert(\_:replacementRange:) 

Instance Method

# insert(\_:replacementRange:)

Inserts an adaptive image into the text at the specifed location.

macOS 15.0+

``` source
optional func insert(
    _ adaptiveImageGlyph: NSAdaptiveImageGlyph,
    replacementRange: NSRange
)
```

## Parameters 

`adaptiveImageGlyph`  

The adaptive image to add to the text.

`replacementRange`  

The text range at which to insert the image.

## See Also

### Supporting adaptive images

var supportsAdaptiveImageGlyph: Bool

A Boolean value that indicates whether the document supports adaptive images in the input.

