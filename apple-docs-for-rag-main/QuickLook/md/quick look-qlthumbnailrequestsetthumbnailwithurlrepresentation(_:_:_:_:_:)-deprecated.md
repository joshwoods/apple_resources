

- Quick Look
-  QLThumbnailRequestSetThumbnailWithURLRepresentation(\_:\_:\_:\_:\_:) Deprecated

Function

# QLThumbnailRequestSetThumbnailWithURLRepresentation(\_:\_:\_:\_:\_:)

Sets the default image representation for an item of a given type at the specified URL.

macOS 10.6–12.0Deprecated

``` source
func QLThumbnailRequestSetThumbnailWithURLRepresentation(
    _ thumbnail: QLThumbnailRequest!,
    _ url: CFURL!,
    _ contentTypeUTI: CFString!,
    _ previewProperties: CFDictionary!,
    _ properties: CFDictionary!
)
```

Deprecated

Use a QLThumbnailReply in a Thumbnail Extension to provide thumbnails for your file types.

## Parameters 

`thumbnail`  

The thumbnail request object.

`url`  

The url to the file of the preview response.

`contentTypeUTI`  

The UTI of the content for the preview representation.

`previewProperties`  

Additional properties for the preview response.

`properties`  

A dictionary of properties for the thumbnail. macOS doesn’t support any properties.

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

func QLThumbnailRequestSetImageWithData(QLThumbnailRequest!, CFData!, CFDictionary!)

Sets the response to the thumbnail request to image data saved within the document.

Deprecated

func QLThumbnailRequestSetThumbnailWithDataRepresentation(QLThumbnailRequest!, CFData!, CFString!, CFDictionary!, CFDictionary!)

Sets the default image representation for an item with the provided data and specified file type.

Deprecated

