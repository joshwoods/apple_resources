

- AVFoundation
- AVCaptureOutput
-  connection(with:) 

Instance Method

# connection(with:)

Returns the first connection with an input port of a specified media type.

iOS 5.0+iPadOS 5.0+Mac Catalyst 14.0+macOS 10.7+tvOS 17.0+visionOS 1.0+

``` source
func connection(with mediaType: AVMediaType) -> AVCaptureConnection?
```

## Parameters 

`mediaType`  

A media type such as video or audio.

## Return Value

The first capture connection that has the specified media type, or `nil` if no connection for the media type exists.

## See Also

### Accessing Connections

var connections: [AVCaptureConnection]

The capture output object’s connections.

enum DataDroppedReason

Constants that define reasons for why the system dropped a frame.

