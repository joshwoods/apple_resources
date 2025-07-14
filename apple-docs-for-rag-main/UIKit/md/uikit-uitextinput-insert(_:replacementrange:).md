

- UIKit
- UITextInput
-  insert(\_:replacementRange:) 

Instance Method

# insert(\_:replacementRange:)

Inserts an adaptive image into the text at the specifed location.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+tvOS 18.0+visionOS 2.0+

``` source
@MainActor
optional func insert(
    _ adaptiveImageGlyph: NSAdaptiveImageGlyph,
    replacementRange: UITextRange
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

