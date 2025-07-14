

- AppKit
-  NSTextPreview 

Class

# NSTextPreview

A snapshot of the text in your view, which the system uses to create user-visible effects.

macOS 15.2+

``` source
@MainActor
class NSTextPreview
```

## Mentioned in 

Adding Writing Tools support to a custom AppKit view

## Overview

An `NSTextPreview` object provides a static image of your view’s text content that the system can use to create animations. You provide preview objects in response to system requests, such as ones from Writing Tools. In addition to creating an image of your view’s text, you also specify the location of that text in your view’s frame rectangle. When creating animations, the system places the image on top of your view’s content and animates changes to the image instead of to your view.

Create an `NSTextPreview` object in response to specific system requests. Create an image with a transparent background and render your view’s text into the image using the current text attributes. Construct your `NSTextPreview` object with both the image and the frame rectangle that represents the location of the rendered text in your view’s coordinate system. To highlight specific portions of text, instead of all the text in the image, provide a set of candidate rectangles with the locations of the text you want to highlight.

## Topics

### Creating a text preview

convenience init(snapshotImage: CGImage, presentationFrame: NSRect)

Creates a text preview using the specified image.

init(snapshotImage: CGImage, presentationFrame: NSRect, candidateRects: [NSValue])

Creates a text preview using the specified image and rectangles that indicate the portions of text to highlight.

### Getting the preview details

var previewImage: CGImage

The image that contains the requested text from your view.

var presentationFrame: NSRect

The frame rectangle that places the preview image directly over the matching text.

var candidateRects: [NSValue]

Rectangles that define the specific portions of text to highlight.

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
- Sendable

