

- Quick Look Thumbnailing
-  QLThumbnailRepresentation 

Class

# QLThumbnailRepresentation

Information about the thumbnail that the thumbnail generator returns.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+visionOS 1.0+

``` source
class QLThumbnailRepresentation
```

## Overview

QuickLook Thumbnailing is a non-UI framework, so your app doesn’t have to link to either UIKit or AppKit. Quicklook Thumbnailing generates a thumbnail as a Core Graphics image object and makes the thumbnail available as the cgImage property. If an app links to AppKit or UIKit, the thumbnail is available through the nsImage or uiImage properties.

For more information on the different types of thumbnails that QLThumbnailGenerator can create, see QLThumbnailGenerator.Request.RepresentationTypes.

## Topics

### Thumbnail Images

var cgImage: CGImage

A thumbnail in the form of a Core Graphics image object.

var nsImage: NSImage

A thumbnail in the form of an AppKit image object.

var uiImage: UIImage

A thumbnail in the form of a UIKit image object.

var type: QLThumbnailRepresentation.RepresentationType

The type of thumbnail.

var contentRect: CGRect

The rectangle within the thumbnail image of the document that represents its contents.

enum RepresentationType

The different types of thumbnails that you can create.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Thumbnail Generation

Creating Quick Look Thumbnails to Preview Files in Your App

Generate thumbnails of images, text files, PDFs, audio files, videos, and more.

class QLThumbnailGenerator

An object that generates thumbnail images based on provided requirements.

