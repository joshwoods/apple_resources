

- Quick Look
-  QLPreviewRequestCopyURL(\_:) Deprecated

Function

# QLPreviewRequestCopyURL(\_:)

Returns the URL of the document for which a preview is requested.

macOS 10.0–12.0Deprecated

``` source
func QLPreviewRequestCopyURL(_ preview: QLPreviewRequest!) -> Unmanaged!
```

Deprecated

Use a QLPreviewingController in a Preview Extension to provide previews for your file types.

## Parameters 

`preview`  

The preview request object.

## Return Value

The URL identifying the file for which the preview is requested.

## Discussion

This function is thread safe.

## See Also

### Requesting previews

func QLPreviewRequestCopyContentUTI(QLPreviewRequest!) -> Unmanaged&lt;CFString>!

Returns the UTI for the preview request.

Deprecated

func QLPreviewRequestCopyOptions(QLPreviewRequest!) -> Unmanaged&lt;CFDictionary>!

Returns the options specified for the preview request.

Deprecated

func QLPreviewRequestCreateContext(QLPreviewRequest!, CGSize, Bool, CFDictionary!) -> Unmanaged&lt;CGContext>!

Creates a graphics context to draw the preview in.

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

