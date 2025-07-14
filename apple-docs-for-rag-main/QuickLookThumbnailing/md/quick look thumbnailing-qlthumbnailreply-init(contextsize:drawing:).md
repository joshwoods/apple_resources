

- Quick Look Thumbnailing
- QLThumbnailReply
-  init(contextSize:drawing:) 

Initializer

# init(contextSize:drawing:)

Creates a new thumbnail for a custom file type in the given context.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.15+visionOS 1.0+

``` source
convenience init(
    contextSize: CGSize,
    drawing drawingBlock: @escaping (CGContext) -> Bool
)
```

## Parameters 

`contextSize`  

The desired size of the context that you pass to the drawing block. Set this value as close as possible to the QLFileThumbnailRequest class’s maximumSize value and greater than or equal to its minimumSize value.

This parameter indicates the preferred size of the thumbnail. The context’s width or its height matches the `width` or `height` of the maximumSize, or, ideally, both.

The system scales the context size to the QLFileThumbnailRequest class’s scale property. For example, if you pass a `contextSize` of `CGSize(10, 10)` to this method, the size of the context is `(scale * 10, scale * 10)`.

`drawingBlock`  

The context for drawing the thumbnail. The block takes the following parameter:

context  
A context of type doc://com.apple.documentation/documentation/coregraphics/cgbitmapcontext that uses the coordinate system provided by Core Graphics.

Return true if you successfully drew the thumbnail into the context. Return false otherwise.

## Return Value

An initialized reply object for a requested thumbnail.

## Discussion

Use this initializer if you’re drawing the thumbnail using Core Graphics. If you’re using UIKit or AppKit to draw the thumbnail, use the initializer init(contextSize:currentContextDrawing:). The context that this initializer provides uses the coordinate system of Core Graphics.

## See Also

### Creating a Thumbnail

convenience init(contextSize: CGSize, currentContextDrawing: () -> Bool)

Creates a new thumbnail for a custom file type in the current context.

convenience init(imageFileURL: URL)

Creates a new thumbnail for a custom file type using a file at the given URL.

