

- Quick Look Thumbnailing
- QLThumbnailGenerator
- QLThumbnailGenerator.Request
-  QLThumbnailGenerator.Request.RepresentationTypes 

Structure

# QLThumbnailGenerator.Request.RepresentationTypes

The various types of thumbnails that you can request.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+visionOS 1.0+

``` source
struct RepresentationTypes
```

## Overview

Thumbnails come in one of three different types:

icon  
A file icon representation.

lowQualityThumbnail  
A faster to generate version of the thumbnail that may sacrifice quality for speed.

thumbnail  
A high-quality thumbnail.

To request all thumbnail representations, use all.

## Topics

### Creating a Thumbnail Type

init(rawValue: UInt)

Creates a new thumbnail type object for a given value.

static var all: QLThumbnailGenerator.Request.RepresentationTypes

The thumbnail type to generate all possible thumbnail representations.

static var icon: QLThumbnailGenerator.Request.RepresentationTypes

A file icon representation of a file.

static var lowQualityThumbnail: QLThumbnailGenerator.Request.RepresentationTypes

A faster to generate version of the thumbnail that may sacrifice quality for speed.

static var thumbnail: QLThumbnailGenerator.Request.RepresentationTypes

A thumbnail representation of a file.

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- ExpressibleByArrayLiteral
- OptionSet
- RawRepresentable
- Sendable
- SetAlgebra

## See Also

### Describing the Requested Thumbnail

var size: CGSize

The size of the thumbnails.

var scale: CGFloat

The pixel density of the display on the intended device.

var contentType: UTType!

The content type of the source data for the thumbnail request.

var representationTypes: QLThumbnailGenerator.Request.RepresentationTypes

The thumbnail sizes that you provide for a thumbnail request.

var minimumDimension: CGFloat

The minimum height or width for a generated thumbnail.

var iconMode: Bool

A Boolean value indicating whether the generated thumbnail request should include icon decorations.

