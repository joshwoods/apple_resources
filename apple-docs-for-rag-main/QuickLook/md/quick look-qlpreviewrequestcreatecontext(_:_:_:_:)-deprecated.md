

- Quick Look
-  QLPreviewRequestCreateContext(\_:\_:\_:\_:) Deprecated

Function

# QLPreviewRequestCreateContext(\_:\_:\_:\_:)

Creates a graphics context to draw the preview in.

macOS 10.0–12.0Deprecated

``` source
func QLPreviewRequestCreateContext(
    _ preview: QLPreviewRequest!,
    _ size: CGSize,
    _ isBitmap: Bool,
    _ properties: CFDictionary!
) -> Unmanaged!
```

Deprecated

Use a QLPreviewingController in a Preview Extension to provide previews for your file types.

## Parameters 

`preview`  

The preview request object.

`size`  

The size of the preview; if `isBitmap` is `true` the size is in pixels, otherwise it’s in points.

`isBitmap`  

`true` if the preview uses a bitmap-based graphics context, `false` otherwise. This value of this parameter affects the interpretation of the `size` parameter.

`properties`  

A dictionary containing properties for the preview response. `Preview Properties` lists the current property keys and describes their values.

## Return Value

A Core Graphics graphics-context object that you can draw your preview image in. You should explicitly release this object when it is no longer needed.

## Discussion

You can directly draw your preview data in the graphics-context object created by this function. After calling this function, you should flush the context with QLPreviewRequestFlushContext(_:_:). Also be sure to release the `CGContext` object.

Quick Look provides three types of graphics contexts for drawing previews: bitmap, single-page vector-based, and multi-page vector-based (for PDF previews). You use this function to acquire a context for bitmap and single-page vector drawing; the `isBitmap` parameter is used to distinguish between them. For multi-page contexts, use the QLPreviewRequestCreatePDFContext(_:_:_:_:) function.

If you prefer to work in Objective-C code, you can convert the created CGContext to a NSGraphicsContext object using init(graphicsPort:flipped:).

### Special Considerations

Thread-safety: This function should be called in the same thread as the preview request is made in; generally, this is the same thread in which the `GeneratePreviewForURL` callback was invoked.

## See Also

### Requesting previews

func QLPreviewRequestCopyContentUTI(QLPreviewRequest!) -> Unmanaged&lt;CFString>!

Returns the UTI for the preview request.

Deprecated

func QLPreviewRequestCopyOptions(QLPreviewRequest!) -> Unmanaged&lt;CFDictionary>!

Returns the options specified for the preview request.

Deprecated

func QLPreviewRequestCopyURL(QLPreviewRequest!) -> Unmanaged&lt;CFURL>!

Returns the URL of the document for which a preview is requested.

Deprecated

func QLPreviewRequestCreatePDFContext(QLPreviewRequest!, UnsafePointer&lt;CGRect>!, CFDictionary!, CFDictionary!) -> Unmanaged&lt;CGContext>!

Creates a PDF context suitable to draw a multi-page preview.

Deprecated

func QLPreviewRequestFlushContext(QLPreviewRequest!, CGContext!)

Flush the context and sets the preview response.

Deprecated

func QLPreviewRequestGetDocumentObject(QLPreviewRequest!) -> UnsafeRawPointer!

Returns the object that’s stored as part of a preview request.

Deprecated

func QLPreviewRequestSetDocumentObject(QLPreviewRequest!, UnsafeRawPointer!, UnsafePointer&lt;CFArrayCallBacks>!)

Stores an object as part of a preview request.

Deprecated

func QLPreviewRequestGetGeneratorBundle(QLPreviewRequest!) -> Unmanaged&lt;CFBundle>!

Get the bundle of the generator receiving the preview request.

Deprecated

func QLPreviewRequestGetTypeID() -> CFTypeID

Gets the type identifier for the `QLPreviewReqest` opaque type.

Deprecated

func QLPreviewRequestIsCancelled(QLPreviewRequest!) -> Bool

Returns whether the preview request has been cancelled by the client.

Deprecated

func QLPreviewRequestSetDataRepresentation(QLPreviewRequest!, CFData!, CFString!, CFDictionary!)

Sets the preview request to data saved within the document or to dynamically generated data.

Deprecated

func QLPreviewRequestSetURLRepresentation(QLPreviewRequest!, CFURL!, CFString!, CFDictionary!)

Sets the contents of the file at the given URL as the response to the preview request.

Deprecated

