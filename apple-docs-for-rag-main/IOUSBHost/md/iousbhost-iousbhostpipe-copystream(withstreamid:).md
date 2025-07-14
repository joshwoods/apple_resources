

- IOUSBHost
- IOUSBHostPipe
-  copyStream(withStreamID:) 

Instance Method

# copyStream(withStreamID:)

Returns the stream for a stream ID.

Mac Catalyst 14.0+macOS 10.15+

``` source
func copyStream(withStreamID streamID: Int) throws -> IOUSBHostStream
```

## Parameters 

`streamID`  

A stream ID in the range of 1 to *n*. Retrieve *n* can by calling IOUSBGetEndpointMaxStreams(_:_:_:) with the IOUSBEndpointDescriptor.

## Return Value

A pointer to an IOUSBHostStream; otherwise, `nil` if the device or the underlying host controller doesn’t support the specified stream ID.

## Discussion

Call enableStreams() before this method.

## See Also

### Managing Streams

func enableStreams() throws

Enables streams for the pipe.

func disableStreams() throws

Disables streams for the pipe.

