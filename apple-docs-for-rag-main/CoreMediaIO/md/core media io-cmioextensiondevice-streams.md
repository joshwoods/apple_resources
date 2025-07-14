

- Core Media I/O
- CMIOExtensionDevice
-  streams 

Instance Property

# streams

An array of media streams attached to this device.

Mac Catalyst 15.4+macOS 12.3+

``` source
var streams: [CMIOExtensionStream] { get }
```

## Discussion

This property isn’t key-value observable.

## See Also

### Managing Streams

func addStream(CMIOExtensionStream) throws

Adds a stream to a device.

func removeStream(CMIOExtensionStream) throws

Removes a stream from the device.

