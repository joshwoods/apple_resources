

- Core Media
- CMTaggedBuffer
-  init(tags:buffer:) 

Initializer

# init(tags:buffer:)

Creates a new tagged buffer from tags and an existing media buffer.

iOS 17.0+iPadOS 17.0+Mac CatalystmacOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
init(
    tags: [CMTag],
    buffer: CMTaggedBuffer.Buffer
)
```

## Parameters 

`tags`  

The tags to assign to the buffer.

`buffer`  

The buffer, wrapped as a CMTaggedBuffer.Buffer, to associate with the tags.

## See Also

### Creating Tagged Buffers

init(tags: [CMTag], sampleBuffer: CMSampleBuffer)

Creates a new tagged buffer from tags and an existing sample buffer.

init(tags: [CMTag], pixelBuffer: CVPixelBuffer)

Creates a new tagged buffer from tags and an existing pixel buffer.

