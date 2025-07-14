

- AVFoundation
- AVAssetImageGenerator
-  AVAssetImageGenerator.Images 

Structure

# AVAssetImageGenerator.Images

An asynchronous sequence of images created by an image generator.

iOS 16.0+iPadOS 16.0+Mac CatalystmacOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
struct Images
```

## Mentioned in 

Creating images from a video asset

## Topics

### Creating an Iterator

func makeAsyncIterator() -> AVAssetImageGenerator.Images

Creates an asynchronous iterator that produces elements of this type.

### Iterating Elements

func next() async -> AVAssetImageGenerator.Images.Element?

Returns the next element in the sequence.

enum Element

An element that provides the result of an image generation request.

## Relationships

### Conforms To

- AsyncIteratorProtocol
- AsyncSequence

