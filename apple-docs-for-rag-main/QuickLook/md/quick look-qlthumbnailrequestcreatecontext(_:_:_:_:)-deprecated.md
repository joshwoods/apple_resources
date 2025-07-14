

- Quick Look
-  QLThumbnailRequestCreateContext(\_:\_:\_:\_:) Deprecated

Function

# QLThumbnailRequestCreateContext(\_:\_:\_:\_:)

Creates a graphics context to draw the thumbnail in.

macOS 10.0–12.0Deprecated

``` source
func QLThumbnailRequestCreateContext(
    _ thumbnail: QLThumbnailRequest!,
    _ size: CGSize,
    _ isBitmap: Bool,
    _ properties: CFDictionary!
) -> Unmanaged!
```

Deprecated

Use a QLThumbnailReply in a Thumbnail Extension to provide thumbnails for your file types.

## Parameters 

`size`  

The size of the thumbnail; if `isBitmap` is `true` the size is in pixels, otherwise it’s in points.

`isBitmap`  

`true` if the thumbnail data is bitmap-based, `false` if vector-based. This value of this parameter affects the interpretation of the `size` parameter.

`properties`  

A dictionary containing properties for the thumbnail response. For macOS 10.5, no properties have been defined.

## Return Value

A Core Graphics graphics-context object that you can draw your thumbnail image in. You should explicitly release this object when it is no longer needed.

## Discussion

You can directly draw your thumbnail data in the graphics-context object created by this function. After calling this function, you should flush the context with QLThumbnailRequestFlushContext(_:_:). Also be sure to release the `CGContext` object.

With this function you can create two types of graphics contexts for drawing thumbnails: bitmap and single-page vector-based; you use the `isBitmap` flag to distinguish between the two. Quick Look handles bitmap thumbnail context differently than non-bitmap contexts; in the latter case, Quick Look might scale the drawing up or down if necessary, and it respects the scale factor (for HiDPI support).

If you prefer to work in Objective-C code, you can convert the created CGContext to a NSGraphicsContext object using init(graphicsPort:flipped:).

### Special Considerations

Thread-safety: This function should be called in the same thread as the thumbnail request is made in; generally, this is the same thread in which the `GenerateThumbnailForURL` callback was invoked.

## See Also

### Handling thumbnail requests

func QLThumbnailRequestCopyContentUTI(QLThumbnailRequest!) -> Unmanaged&lt;CFString>!

Returns the UTI for the thumbnail request.

Deprecated

func QLThumbnailRequestCopyOptions(QLThumbnailRequest!) -> Unmanaged&lt;CFDictionary>!

Returns the options specified for the thumbnail request.

Deprecated

func QLThumbnailRequestCopyURL(QLThumbnailRequest!) -> Unmanaged&lt;CFURL>!

Returns the URL of the document for which the thumbnail request is requested.

Deprecated

func QLThumbnailRequestFlushContext(QLThumbnailRequest!, CGContext!)

Flush the graphics context and sets the thumbnail response.

Deprecated

func QLThumbnailRequestGetDocumentObject(QLThumbnailRequest!) -> UnsafeRawPointer!

Returns the object that’s stored as part of a thumbnail request.

Deprecated

func QLThumbnailRequestGetGeneratorBundle(QLThumbnailRequest!) -> Unmanaged&lt;CFBundle>!

Get the bundle of the generator receiving the thumbnail request.

Deprecated

func QLThumbnailRequestGetMaximumSize(QLThumbnailRequest!) -> CGSize

Returns the maximum size (in points) specified for the thumbnail image.

Deprecated

func QLThumbnailRequestGetTypeID() -> CFTypeID

Gets the type identifier for the `QLThumbnailRequest` opaque type.

Deprecated

func QLThumbnailRequestIsCancelled(QLThumbnailRequest!) -> Bool

Returns whether the thumbnail request has been cancelled by the client.

Deprecated

func QLThumbnailRequestSetDocumentObject(QLThumbnailRequest!, UnsafeRawPointer!, UnsafePointer&lt;CFArrayCallBacks>!)

Stores an object as part of a thumbnail request.

Deprecated

func QLThumbnailRequestSetImage(QLThumbnailRequest!, CGImage!, CFDictionary!)

Sets the thumbnail request to a specified image.

Deprecated

func QLThumbnailRequestSetImageAtURL(QLThumbnailRequest!, CFURL!, CFDictionary!)

Sets the thumbnail request to contain the image at a given URL.

Deprecated

func QLThumbnailRequestSetImageWithData(QLThumbnailRequest!, CFData!, CFDictionary!)

Sets the response to the thumbnail request to image data saved within the document.

Deprecated

func QLThumbnailRequestSetThumbnailWithDataRepresentation(QLThumbnailRequest!, CFData!, CFString!, CFDictionary!, CFDictionary!)

Sets the default image representation for an item with the provided data and specified file type.

Deprecated

func QLThumbnailRequestSetThumbnailWithURLRepresentation(QLThumbnailRequest!, CFURL!, CFString!, CFDictionary!, CFDictionary!)

Sets the default image representation for an item of a given type at the specified URL.

Deprecated

