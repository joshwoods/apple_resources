

- Quick Look
-  QLPreviewRequestSetDataRepresentation(\_:\_:\_:\_:) Deprecated

Function

# QLPreviewRequestSetDataRepresentation(\_:\_:\_:\_:)

Sets the preview request to data saved within the document or to dynamically generated data.

macOS 10.0–12.0Deprecated

``` source
func QLPreviewRequestSetDataRepresentation(
    _ preview: QLPreviewRequest!,
    _ data: CFData!,
    _ contentTypeUTI: CFString!,
    _ properties: CFDictionary!
)
```

Deprecated

Use a QLPreviewingController in a Preview Extension to provide previews for your file types.

## Parameters 

`preview`  

The preview request object.

`data`  

The data of the preview returned to the client.

`contentTypeUTI`  

The UTI specifying the content type of the preview.

`properties`  

Additional properties for the preview response. For more on supported keys and values for this dictionary, see `Preview Properties`. If the saved data is HTML, you may specify a special set of properties; see the discussion below for more information.

## Discussion

This function returns preview data to the client. The data is either extracted from a document where the document’s application has saved it, or it’s dynamically generated. How Quick Look handles the data depends upon the value of `contentTypeUTI`. The content data of the preview must be of a native Quick Look type. Currently supported UTIs for these types are: `kUTTypeImage`, `kUTTypePDF`, `kUTTypeHTML`, `kUTTypeXML`, `kUTTypePlainText`, `kUTTypeRTF`, `kUTTypeMovie`, and `kUTTypeAudio`.

If the UTI type is `kUTTypeHTML`, you can have WebKit handle the layout and display of your preview. You must provide the HTML in `data` plus any attachments (for example, Address Book cards, Mail messages, or Omni Outliner documents) in the `properties` dictionary. This dictionary takes kQLPreviewPropertyAttachmentsKey as its key and consists of one ore more subdictionaries (one per attachment). Each subdictionary uses an arbitrary string identifier as a key; the attachment should be referenced within the HTML data using the kQLPreviewContentIDScheme URL scheme (“cid”) and the identifier as the URL resource specifier—for example, “cid:the_identifier”. The keys of the subdictionary properties are kQLPreviewPropertyMIMETypeKey, kQLPreviewPropertyTextEncodingNameKey, and kQLPreviewPropertyAttachmentDataKey.

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

func QLPreviewRequestSetURLRepresentation(QLPreviewRequest!, CFURL!, CFString!, CFDictionary!)

Sets the contents of the file at the given URL as the response to the preview request.

Deprecated

