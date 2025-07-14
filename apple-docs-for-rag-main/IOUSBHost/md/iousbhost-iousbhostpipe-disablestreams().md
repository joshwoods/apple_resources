

- IOUSBHost
- IOUSBHostPipe
-  disableStreams() 

Instance Method

# disableStreams()

Disables streams for the pipe.

Mac Catalyst 14.0+macOS 10.15+

``` source
func disableStreams() throws
```

## Discussion

This method changes the operational mode of the IOUSBHostPipe to disable streaming endpoint transfers. Before calling this method, set all stream contexts as nonactive on the device through an out-of-band (class-defined) mechanism, in accordance with USB 3.2, 8.12.1.4. This is necessary, as the method synchronously aborts any outstanding calls on existing IOUSBHostStream objects.

## See Also

### Managing Streams

func enableStreams() throws

Enables streams for the pipe.

func copyStream(withStreamID: Int) throws -> IOUSBHostStream

Returns the stream for a stream ID.

