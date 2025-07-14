

- Quick Look
-  QLPreviewRequestCreatePDFContext(\_:\_:\_:\_:) Deprecated

Function

# QLPreviewRequestCreatePDFContext(\_:\_:\_:\_:)

Creates a PDF context suitable to draw a multi-page preview.

macOS 10.0–12.0Deprecated

``` source
func QLPreviewRequestCreatePDFContext(
    _ preview: QLPreviewRequest!,
    _ mediaBox: UnsafePointer!,
    _ auxiliaryInfo: CFDictionary!,
    _ properties: CFDictionary!
) -> Unmanaged!
```

Deprecated

Use a QLPreviewingController in a Preview Extension to provide previews for your file types.

## Parameters 

`preview`  

The preview request object.

`mediaBox`  

A pointer to the media box of the context.

A media box is a rectangle that defines the size and location of the PDF page. The origin of the rectangle should typically be (0,0). If you pass NULL, Quartz uses a default page size of 8.5 by 11 inches (612 by 792 points). For information see the description for init(consumer:mediaBox:_:).

`auxiliaryInfo`  

A dictionary containing PDF auxiliary information. See the description of the auxiliary dictionary keys in doc://com.apple.documentation/documentation/coregraphics/cgpdfcontext for more information about the keys and values of this dictionary.

`properties`  

A dictionary containing additional properties for the preview response. For information on acceptable keys and values, see `Preview Properties`.

## Return Value

A reference to a Core Graphics context object that is used to display a PDF version of the preview. You should explicitly release this object when it is no longer needed.

## Discussion

Be sure to bracket each PDF page written to the context with beginPDFPage(_:) and endPDFPage() calls. After calling this function, you should flush the context with QLPreviewRequestFlushContext(_:_:).

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

func QLPreviewRequestCreateContext(QLPreviewRequest!, CGSize, Bool, CFDictionary!) -> Unmanaged&lt;CGContext>!

Creates a graphics context to draw the preview in.

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

