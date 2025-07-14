

- Core Media
-  CMTaggedBuffer 

Structure

# CMTaggedBuffer

An instance of a media buffer containing metadata tags.

iOS 17.0+iPadOS 17.0+Mac CatalystmacOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
struct CMTaggedBuffer
```

## Topics

### Creating Tagged Buffers

init(tags: [CMTag], buffer: CMTaggedBuffer.Buffer)

Creates a new tagged buffer from tags and an existing media buffer.

init(tags: [CMTag], sampleBuffer: CMSampleBuffer)

Creates a new tagged buffer from tags and an existing sample buffer.

init(tags: [CMTag], pixelBuffer: CVPixelBuffer)

Creates a new tagged buffer from tags and an existing pixel buffer.

### Inspecting Data

let tags: [CMTag]

The tags for this buffer.

let buffer: CMTaggedBuffer.Buffer

The underlying buffer containing media data.

### Buffer Wrappers

enum Buffer

A wrapper type for the underlying buffer of a tagged buffer.

## Relationships

### Conforms To

- CustomStringConvertible

## See Also

### Sample Processing

CMSampleBuffer APIs

An object that contains zero or more media samples of a uniform media type.

CMBlockBuffer APIs

An object the system uses to move blocks of memory through a processing system.

CMTaggedBufferGroup APIs

Objective-C types and interfaces for working with Core Media tagged buffer groups.

CMFormatDescription APIs

A media format descriptor that describes the samples in a sample buffer.

CMAttachment APIs

Add supporting metadata to sample buffers.

