

- Quick Look
-  kQLPreviewPropertyBaseBundlePathKey Deprecated

Global Variable

# kQLPreviewPropertyBaseBundlePathKey

A path that’s outside of the default security scope for creating a preview.

macOS 10.6–12.0Deprecated

``` source
let kQLPreviewPropertyBaseBundlePathKey: CFString!
```

Deprecated

Use a QLPreviewingController in a Preview Extension to provide previews for your file types.

## Discussion

By default, the Quick Look feature only accepts files within the current document bundle. Use `kQLPreviewPropertyBaseBundlePathKey` to expand the accepted security scope and look at files outside of the current document bundle. The associated value is a path as a doc://com.apple.documentation/documentation/corefoundation/cfstring-rfh.

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

