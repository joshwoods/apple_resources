

- Core Media
- CMTaggedBuffer
-  init(tags:sampleBuffer:) 

Initializer

# init(tags:sampleBuffer:)

Creates a new tagged buffer from tags and an existing sample buffer.

iOS 17.0+iPadOS 17.0+Mac CatalystmacOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
init(
    tags: [CMTag],
    sampleBuffer: CMSampleBuffer
)
```

## Parameters 

`tags`  

The tags to assign to the buffer.

`sampleBuffer`  

A sample buffer to associate with the tags.

## See Also

### Creating Tagged Buffers

init(tags: [CMTag], buffer: CMTaggedBuffer.Buffer)

Creates a new tagged buffer from tags and an existing media buffer.

init(tags: [CMTag], pixelBuffer: CVPixelBuffer)

Creates a new tagged buffer from tags and an existing pixel buffer.

