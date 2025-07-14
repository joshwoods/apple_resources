

- Core Media
- CMSampleBuffer
-  dataReadiness 

Instance Property

# dataReadiness

A value that indicates the status of the data the sample buffer contains.

iOS 13.0+iPadOS 13.0+Mac CatalystmacOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
var dataReadiness: CMSampleBuffer.DataReadiness { get }
```

## See Also

### Determining Readiness

func setDataReadiness(CMSampleBuffer.DataReadiness) throws

Sets the status of the sample buffer’s data.

enum DataReadiness

Constants that indicate the readiness of a sample buffer’s data.

func makeDataReady() throws

Makes the sample buffer’s data ready for use by calling its handler closure.

func trackDataReadiness(CMSampleBuffer) throws

Associates a sample buffer’s data readiness with that of another sample buffer.

