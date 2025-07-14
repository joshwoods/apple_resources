

- Core Media
- CMTaggedBuffer
-  CMTaggedBuffer.Buffer 

Enumeration

# CMTaggedBuffer.Buffer

A wrapper type for the underlying buffer of a tagged buffer.

iOS 17.0+iPadOS 17.0+Mac CatalystmacOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
enum Buffer
```

## Topics

### Wrapped Buffer Types

case pixelBuffer(CVPixelBuffer)

The underlying pixel buffer for a tagged buffer.

case sampleBuffer(CMSampleBuffer)

The underlying sample buffer for a tagged buffer.

