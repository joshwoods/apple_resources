

- Core Media I/O
- CMIOExtensionDevice
-  addStream(\_:) 

Instance Method

# addStream(\_:)

Adds a stream to a device.

Mac Catalyst 15.4+macOS 12.3+

``` source
func addStream(_ stream: CMIOExtensionStream) throws
```

## Parameters 

`stream`  

A stream to add to a device.

## See Also

### Managing Streams

var streams: [CMIOExtensionStream]

An array of media streams attached to this device.

func removeStream(CMIOExtensionStream) throws

Removes a stream from the device.

