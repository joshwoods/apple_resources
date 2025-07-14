

- Image Playground
- ImageCreator
-  ImageCreator.CreatedImage 

Structure

# ImageCreator.CreatedImage

A structure that stores a programmatically generated image.

iOS 18.4+iPadOS 18.4+Mac Catalyst 18.4+macOS 15.4+visionOS 2.4+

``` source
struct CreatedImage
```

## Overview

You receive `CreatedImage` structures from an `ImageCreator` object when you ask that object to generate images for you. You cannot create instances of this structure yourself.

## Topics

### Getting the image

let cgImage: CGImage

The programmatically generated image.

## See Also

### Generating images

func images(for: [ImagePlaygroundConcept], style: ImagePlaygroundStyle, limit: Int) -> some AsyncSequence&lt;ImageCreator.CreatedImage, any Error> 

Starts the creation of images based on the description and style information you provide.

let availableStyles: [ImagePlaygroundStyle]

The set of styles you can apply to the images you create.

enum Error

Errors that can occur during the image generation process.

