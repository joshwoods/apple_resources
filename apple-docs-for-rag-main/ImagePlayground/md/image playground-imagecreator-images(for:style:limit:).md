

- Image Playground
- ImageCreator
-  images(for:style:limit:) 

Instance Method

# images(for:style:limit:)

Starts the creation of images based on the description and style information you provide.

iOS 18.4+iPadOS 18.4+Mac Catalyst 18.4+macOS 15.4+visionOS 2.4+

``` source
final func images(
    for concepts: [ImagePlaygroundConcept],
    style: ImagePlaygroundStyle,
    limit: Int
) -> some AsyncSequence
```

## Parameters 

`concepts`  

The elements that describe the expected contents of the image.

`style`  

The style you want the model to apply to the output image. It is a programmer error to specify a style that’s not in the `availableStyles` property.

`limit`  

The maximum number of images you want the system to create. The system limits the maximum number of images to 4.

## Return Value

An asynchronous stream you use to receive the images.

## Discussion

Call this method to start the image generation process with the specified parameters. The method executes asynchronously and returns the images on the provided AsyncSequence object. The following example configures an image creator, starts the creation of the images, and processes the generated images as they arrive.

```
```

## See Also

### Generating images

let availableStyles: [ImagePlaygroundStyle]

The set of styles you can apply to the images you create.

struct CreatedImage

A structure that stores a programmatically generated image.

enum Error

Errors that can occur during the image generation process.

