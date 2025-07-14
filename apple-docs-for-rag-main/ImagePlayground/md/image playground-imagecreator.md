

- Image Playground
-  ImageCreator 

Class

# ImageCreator

Generates images programmatically from the description and style information you specify.

iOS 18.4+iPadOS 18.4+Mac Catalyst 18.4+macOS 15.4+visionOS 2.4+

``` source
final class ImageCreator
```

## Overview

Use an `ImageCreator` object to generate images programmatically from your app on devices that support the capability. You provide a description of the image content, as a text string or as a combination of text and images. The system’s generative models use that information to generate one or more images and return them to your code.

Create an `ImageCreator` object and use its images(for:style:limit:) method to start the image generation process. Image generation occurs asynchronously, delivering results back to your code using an AsyncSequence object.

## Topics

### Creating the object

init() async throws

Creates a new image creator object for you to use in your app.

### Generating images

func images(for: [ImagePlaygroundConcept], style: ImagePlaygroundStyle, limit: Int) -> some AsyncSequence&lt;ImageCreator.CreatedImage, any Error> 

Starts the creation of images based on the description and style information you provide.

let availableStyles: [ImagePlaygroundStyle]

The set of styles you can apply to the images you create.

struct CreatedImage

A structure that stores a programmatically generated image.

enum Error

Errors that can occur during the image generation process.

## Relationships

### Conforms To

- Sendable

