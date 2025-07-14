

- Quick Look
-  QLThumbnailRequestCopyOptions(\_:) Deprecated

Function

# QLThumbnailRequestCopyOptions(\_:)

Returns the options specified for the thumbnail request.

macOS 10.0–12.0Deprecated

``` source
func QLThumbnailRequestCopyOptions(_ thumbnail: QLThumbnailRequest!) -> Unmanaged!
```

Deprecated

Use a QLFileThumbnailRequest in a Thumbnail Extension to provide thumbnails for your file types.

## Parameters 

`thumbnail`  

A thumbnail request object.

## Return Value

A dictionary containing the options that the client specified for the thumbnail request. See `General Thumbnail Options` for supported options. You should explicitly release the dictionary when it is no longer needed.

## Discussion

The client sets options in the thumbnail request to give hints to the generator. For macOS 10.5, no options are supported. You should explicitly release the dictionary when it’s no longer needed.

### Special Considerations

Thread-safety: This function should be called in the same thread as the thumbnail request is made in; generally, this is the same thread in which the `GenerateThumbnailForURL` callback was invoked.

## See Also

### Handling thumbnail requests

func QLThumbnailRequestCopyContentUTI(QLThumbnailRequest!) -> Unmanaged&lt;CFString>!

Returns the UTI for the thumbnail request.

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

func QLThumbnailRequestSetImageWithData(QLThumbnailRequest!, CFData!, CFDictionary!)

Sets the response to the thumbnail request to image data saved within the document.

Deprecated

func QLThumbnailRequestSetThumbnailWithDataRepresentation(QLThumbnailRequest!, CFData!, CFString!, CFDictionary!, CFDictionary!)

Sets the default image representation for an item with the provided data and specified file type.

Deprecated

func QLThumbnailRequestSetThumbnailWithURLRepresentation(QLThumbnailRequest!, CFURL!, CFString!, CFDictionary!, CFDictionary!)

Sets the default image representation for an item of a given type at the specified URL.

Deprecated

