

- Image Playground
- ImageCreator
-  availableStyles 

Instance Property

# availableStyles

The set of styles you can apply to the images you create.

iOS 18.4+iPadOS 18.4+Mac Catalyst 18.4+macOS 15.4+visionOS 2.4+

``` source
final let availableStyles: [ImagePlaygroundStyle]
```

## Discussion

Before requesting any images, make sure the style you want to use is in this property.

## See Also

### Generating images

func images(for: [ImagePlaygroundConcept], style: ImagePlaygroundStyle, limit: Int) -> some AsyncSequence&lt;ImageCreator.CreatedImage, any Error> 

Starts the creation of images based on the description and style information you provide.

struct CreatedImage

A structure that stores a programmatically generated image.

enum Error

Errors that can occur during the image generation process.

