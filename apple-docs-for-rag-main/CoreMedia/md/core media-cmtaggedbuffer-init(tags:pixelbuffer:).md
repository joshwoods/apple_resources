

- Core Media
- CMTaggedBuffer
-  init(tags:pixelBuffer:) 

Initializer

# init(tags:pixelBuffer:)

Creates a new tagged buffer from tags and an existing pixel buffer.

iOS 17.0+iPadOS 17.0+Mac CatalystmacOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
init(
    tags: [CMTag],
    pixelBuffer: CVPixelBuffer
)
```

## Parameters 

`tags`  

The tags to assign to the buffer.

`pixelBuffer`  

A pixel buffer containing image-based media to associate with the tags.

## See Also

### Creating Tagged Buffers

init(tags: [CMTag], buffer: CMTaggedBuffer.Buffer)

Creates a new tagged buffer from tags and an existing media buffer.

init(tags: [CMTag], sampleBuffer: CMSampleBuffer)

Creates a new tagged buffer from tags and an existing sample buffer.

