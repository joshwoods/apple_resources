

- Image Playground
-  ImagePlaygroundConcept 

Structure

# ImagePlaygroundConcept

Text elements that specify the content to include in the image.

iOS 18.1+iPadOS 18.1+Mac Catalyst 18.1+macOS 15.1+visionOS 2.4+

``` source
struct ImagePlaygroundConcept
```

## Overview

Use this type to wrap pieces of text describing the image you want to create. You can also specify larger pieces of text that contain important concepts to extract and use to guide the image-creation process.

## Topics

### Describing the image

static func text(String) -> ImagePlaygroundConcept

Creates a concept structure that includes a short text description.

static func extracted(from: String, title: String?) -> ImagePlaygroundConcept

Creates a concept structure from a long-form string and a title that guides the extraction of concepts from that string.

static func drawing(PKDrawing) -> ImagePlaygroundConcept

Creates a concept structure from a PencilKit drawing.

static func image(CGImage) -> ImagePlaygroundConcept

Creates a concept structure from the specified image object.

static func image(URL) -> ImagePlaygroundConcept?

Creates a concept structure from the image at the specified URL.

### Type Methods

static func extracted(from: String) -> ImagePlaygroundConcept

Builds a playground concept by extracting multiple concepts from a long text that describes the contents of the image.

Deprecated

## See Also

### Platform support

struct ImagePlaygroundStyle

Style options that determine the appearance of generated images.

