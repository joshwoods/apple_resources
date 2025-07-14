

- Quick Look
-  kQLPreviewPropertyStringEncodingKey Deprecated

Global Variable

# kQLPreviewPropertyStringEncodingKey

The string encoding of the preview data.

macOS 10.0–12.0Deprecated

``` source
let kQLPreviewPropertyStringEncodingKey: CFString!
```

Deprecated

Use a QLPreviewingController in a Preview Extension to provide previews for your file types.

## Discussion

Specifies the string encoding of the preview data as an CFStringEncoding if the native type is plain text. You must encapsulate the value in a doc://com.apple.documentation/documentation/corefoundation/cfnumber-rjd object.

## See Also

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

