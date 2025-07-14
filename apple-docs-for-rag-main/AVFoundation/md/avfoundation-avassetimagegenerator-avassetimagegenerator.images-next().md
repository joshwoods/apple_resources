

- AVFoundation
- AVAssetImageGenerator
- AVAssetImageGenerator.Images
-  next() 

Instance Method

# next()

Returns the next element in the sequence.

iOS 16.0+iPadOS 16.0+Mac CatalystmacOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
mutating func next() async -> AVAssetImageGenerator.Images.Element?
```

## Return Value

The next element, or `nil` if no more exist.

## See Also

### Iterating Elements

enum Element

An element that provides the result of an image generation request.

