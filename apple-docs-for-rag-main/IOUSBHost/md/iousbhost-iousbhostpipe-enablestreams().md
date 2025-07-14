

- IOUSBHost
- IOUSBHostPipe
-  enableStreams() 

Instance Method

# enableStreams()

Enables streams for the pipe.

Mac Catalyst 14.0+macOS 10.15+

``` source
func enableStreams() throws
```

## Discussion

This method changes the operational mode of the pipe to allow streaming endpoint transfers. Call this method before copyStream(withStreamID:).

## See Also

### Managing Streams

func copyStream(withStreamID: Int) throws -> IOUSBHostStream

Returns the stream for a stream ID.

func disableStreams() throws

Disables streams for the pipe.

