

- Core Media I/O
- CMIOExtensionDevice
-  removeStream(\_:) 

Instance Method

# removeStream(\_:)

Removes a stream from the device.

Mac Catalyst 15.4+macOS 12.3+

``` source
func removeStream(_ stream: CMIOExtensionStream) throws
```

## Parameters 

`stream`  

The stream to remove from the device.

## See Also

### Managing Streams

var streams: [CMIOExtensionStream]

An array of media streams attached to this device.

func addStream(CMIOExtensionStream) throws

Adds a stream to a device.

