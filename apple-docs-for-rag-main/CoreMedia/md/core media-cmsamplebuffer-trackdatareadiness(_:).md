

- Core Media
- CMSampleBuffer
-  trackDataReadiness(\_:) 

Instance Method

# trackDataReadiness(\_:)

Associates a sample buffer’s data readiness with that of another sample buffer.

iOS 13.0+iPadOS 13.0+Mac CatalystmacOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
func trackDataReadiness(_ sampleBufferToTrack: CMSampleBuffer) throws
```

## Parameters 

`sampleBufferToTrack`  

The sample buffer for which to track readiness.

## Discussion

After calling this method, retrieving the value of the dataReadiness property retrieves the value from the tracked sample buffer. Likewise, calling the makeDataReady() method calls the tracked sample buffers method.

Use this method to convert a multi-sample buffer into single-sample buffer before the data is ready. The single-sample buffer tracks the data readiness of the multi-sample buffers.

## See Also

### Determining Readiness

var dataReadiness: CMSampleBuffer.DataReadiness

A value that indicates the status of the data the sample buffer contains.

func setDataReadiness(CMSampleBuffer.DataReadiness) throws

Sets the status of the sample buffer’s data.

enum DataReadiness

Constants that indicate the readiness of a sample buffer’s data.

func makeDataReady() throws

Makes the sample buffer’s data ready for use by calling its handler closure.

