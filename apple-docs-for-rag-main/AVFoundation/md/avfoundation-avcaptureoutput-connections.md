

- AVFoundation
- AVCaptureOutput
-  connections 

Instance Property

# connections

The capture output object’s connections.

iOS 4.0+iPadOS 4.0+Mac Catalyst 14.0+macOS 10.7+tvOS 17.0+

``` source
var connections: [AVCaptureConnection] { get }
```

## Discussion

Each connection object in the array describes the mapping between the output and the capture input ports.

## See Also

### Accessing Connections

func connection(with: AVMediaType) -> AVCaptureConnection?

Returns the first connection with an input port of a specified media type.

enum DataDroppedReason

Constants that define reasons for why the system dropped a frame.

