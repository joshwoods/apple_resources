

- Core Media
- CMSampleBuffer
-  CMSampleBuffer.DataReadiness 

Enumeration

# CMSampleBuffer.DataReadiness

Constants that indicate the readiness of a sample buffer’s data.

iOS 13.0+iPadOS 13.0+Mac CatalystmacOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
enum DataReadiness
```

## Topics

### States

case notReady

The media data isn’t ready to use.

case ready

The media data is ready to use.

case failed(OSStatus)

The system failed to load the media data.

## Relationships

### Conforms To

- Equatable
- Hashable
- Sendable

## See Also

### Determining Readiness

var dataReadiness: CMSampleBuffer.DataReadiness

A value that indicates the status of the data the sample buffer contains.

func setDataReadiness(CMSampleBuffer.DataReadiness) throws

Sets the status of the sample buffer’s data.

func makeDataReady() throws

Makes the sample buffer’s data ready for use by calling its handler closure.

func trackDataReadiness(CMSampleBuffer) throws

Associates a sample buffer’s data readiness with that of another sample buffer.

