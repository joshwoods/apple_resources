

- Quick Look
-  QLThumbnailRequestSetImageWithData(\_:\_:\_:) Deprecated

Function

# QLThumbnailRequestSetImageWithData(\_:\_:\_:)

Sets the response to the thumbnail request to image data saved within the document.

macOS 10.0–12.0Deprecated

``` source
func QLThumbnailRequestSetImageWithData(
    _ thumbnail: QLThumbnailRequest!,
    _ data: CFData!,
    _ properties: CFDictionary!
)
```

Deprecated

Use a QLThumbnailReply in a Thumbnail Extension to provide thumbnails for your file types.

## Parameters 

`thumbnail`  

The thumbnail request object.

`data`  

The image data, which must be in a format supported by the Image I/O framework (JPG, PNG, and so on). In other words, a content type of `kUTTypeImage` is assumed. (`ImageIO.framework` is a subframework of the umbrella Application Services framework.)

`properties`  

A dictionary of properties. The only property that you can currently specify is kCGImageSourceTypeIdentifierHint; see Quartz 2D Programming Guide for information about this property.

## Discussion

This function returns the thumbnail as a `CFData` object containing image data. The document’s application must save this data as part of the document’s data; the generator retrieves it and uses this function to return it to the client. Before you call this function, call QLThumbnailRequestGetMaximumSize(_:) to obtain the maximum allowed size for the thumbnail and resize the image if necessary.

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

func QLThumbnailRequestCreateContext(QLThumbnailRequest!, CGSize, Bool, CFDictionary!) -> Unmanaged&lt;CGContext>!

Creates a graphics context to draw the thumbnail in.

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

func QLThumbnailRequestSetThumbnailWithDataRepresentation(QLThumbnailRequest!, CFData!, CFString!, CFDictionary!, CFDictionary!)

Sets the default image representation for an item with the provided data and specified file type.

Deprecated

func QLThumbnailRequestSetThumbnailWithURLRepresentation(QLThumbnailRequest!, CFURL!, CFString!, CFDictionary!, CFDictionary!)

Sets the default image representation for an item of a given type at the specified URL.

Deprecated

