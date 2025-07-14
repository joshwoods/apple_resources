

- Quick Look
-  Previews or thumbnail images for macOS 10.14 or earlier 

API Collection

# Previews or thumbnail images for macOS 10.14 or earlier

Create thumbnail images or previews of common files and custom file types in earlier versions of macOS.

## Overview

The Quick Look framework provides functionality to create a miniature representation, or *thumbnail*, of a file and its contents for display in apps that target macOS 10.14 and earlier.

If your app targets macOS 10.15 and later, use the Quick Look Thumbnailing framework to create thumbnails. Similarly, use a Quick Look preview extension to display previews of files instead of Quick Look generators. To learn more, watch What’s New in File Management and Quick Look.

## Topics

### Creating thumbnails

func QLThumbnailImageCreate(CFAllocator!, CFURL!, CGSize, CFDictionary!) -> Unmanaged&lt;CGImage>!

Creates a thumbnail image for the specified file.

Deprecated

func QLThumbnailCreate(CFAllocator!, CFURL!, CGSize, CFDictionary!) -> Unmanaged&lt;QLThumbnail>!

Returns a thumbnail that’s generated in the background.

Deprecated

func QLThumbnailDispatchAsync(QLThumbnail!, dispatch_queue_t!, (() -> Void)!)

Creates a thumbnail in the background on the provided background queue.

Deprecated

func QLThumbnailCancel(QLThumbnail!)

Cancels the computation of the thumbnail.

Deprecated

func QLThumbnailCopyDocumentURL(QLThumbnail!) -> Unmanaged&lt;CFURL>!

Returns the URL of the document that you’re requesting a thumbnail for.

Deprecated

func QLThumbnailCopyImage(QLThumbnail!) -> Unmanaged&lt;CGImage>!

Returns a thumbnail image.

Deprecated

func QLThumbnailCopyOptions(QLThumbnail!) -> Unmanaged&lt;CFDictionary>!

Returns the options for the requested thumbnail.

Deprecated

func QLThumbnailGetContentRect(QLThumbnail!) -> CGRect

Returns the rectangle of the provided thumbnail image that represents the content of the document.

Deprecated

func QLThumbnailGetMaximumSize(QLThumbnail!) -> CGSize

Returns the maximum allowed size for the provided thumbnail image.

Deprecated

func QLThumbnailGetTypeID() -> CFTypeID

Returns the type identifier for the thumbnail’s opaque type.

Deprecated

func QLThumbnailIsCancelled(QLThumbnail!) -> Bool

Returns whether the creation of the thumbnail was canceled.

Deprecated

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

func QLThumbnailRequestSetThumbnailWithURLRepresentation(QLThumbnailRequest!, CFURL!, CFString!, CFDictionary!, CFDictionary!)

Sets the default image representation for an item of a given type at the specified URL.

Deprecated

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

func QLPreviewRequestSetDataRepresentation(QLPreviewRequest!, CFData!, CFString!, CFDictionary!)

Sets the preview request to data saved within the document or to dynamically generated data.

Deprecated

func QLPreviewRequestSetURLRepresentation(QLPreviewRequest!, CFURL!, CFString!, CFDictionary!)

Sets the contents of the file at the given URL as the response to the preview request.

Deprecated

### Configuring the appearance of PDF previews

struct QLPreviewPDFStyle

A value you use to configure the appearance of previews for PDF files.

### Interfacing with a Quick Look plug-in

struct QLGeneratorInterfaceStruct

An opaque reference that provides callbacks that the platform uses to interface with a Quick Look plug-in.

### Opaque types

class QLThumbnail

An opaque reference that represents a thumbnail object.

class QLThumbnailRequest

An opaque reference that represents a thumbnail request object.

class QLPreviewRequest

An opaque reference that represents a preview request object.

### Constants

var kQLReturnMask: Int32

The Quick Look generator can create a preview.

var kQLReturnHasMore: Int32

The Quick Look generator has more content to display as part of the preview.

let kQLThumbnailOptionIconModeKey: CFString!

The Quick Look generator produces the thumbnail as an icon with decor.

let kQLThumbnailOptionScaleFactorKey: CFString!

The scale factor for the thumbnail.

var QUICKLOOK_VERSION: Int32

### Deprecated constants

let kQLPreviewContentIDScheme: CFString!

The content ID URL scheme.

Deprecated

let kQLPreviewPropertyCursorKey: CFString!Deprecated

let kQLPreviewOptionCursorKey: CFString!Deprecated

let kQLPreviewPropertyAttachmentDataKey: CFString!

Attachment data for a preview.

Deprecated

let kQLPreviewPropertyAttachmentsKey: CFString!

A list of attachments or sub-resources.

Deprecated

let kQLPreviewPropertyBaseBundlePathKey: CFString!

A path that’s outside of the default security scope for creating a preview.

Deprecated

let kQLPreviewPropertyDisplayNameKey: CFString!

A custom display name for the preview panel.

Deprecated

let kQLPreviewPropertyHeightKey: CFString!

The height in points of the preview.

Deprecated

let kQLPreviewPropertyMIMETypeKey: CFString!

The web content or attachment mime type.

Deprecated

let kQLPreviewPropertyPDFStyleKey: CFString!

The preferred way to display PDF content.

Deprecated

let kQLPreviewPropertyStringEncodingKey: CFString!

The string encoding of the preview data.

Deprecated

let kQLPreviewPropertyTextEncodingNameKey: CFString!

The encoding of the web content or attachment text.

let kQLPreviewPropertyWidthKey: CFString!

The width in points of the preview.

Deprecated

let kQLThumbnailPropertyBadgeImageKey: CFString!

An image to use for generating the badge for a file’s icon.

Deprecated

let kQLThumbnailPropertyBaseBundlePathKey: CFString!

A path that’s outside of the default security scope for creating a thumbnail.

Deprecated

let kQLThumbnailPropertyExtensionKey: CFString!

The extension to use as a badge when creating an icon.

Deprecated

### QuickLookUI symbols

class QLFilePreviewRequest

class QLPreviewProvider

class QLPreviewReply

class QLPreviewReplyAttachment

protocol QLPreviewItem

protocol QLPreviewingController

For view based previews, the view controller that implements the QLPreviewingController protocol must at least implement one of the two following methods: -\[QLPreviewingController preparePreviewOfSearchableItemWithIdentifier:queryString:completionHandler:\], to generate previews for Spotlight searchable items. -\[QLPreviewingController preparePreviewOfFileAtURL:completionHandler:\], to generate previews for file URLs.

## See Also

### Previews

class QLPreviewController

A specialized view controller for previewing an item.

protocol QLPreviewItem : NSObjectProtocol

A protocol that defines a set of properties you implement to make a preview of your application’s content.

class QLPreviewSceneActivationConfiguration

A scene configuration to preview items at the specified URLs.

