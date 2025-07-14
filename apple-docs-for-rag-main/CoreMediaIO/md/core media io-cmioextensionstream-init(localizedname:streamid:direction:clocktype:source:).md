

- Core Media I/O
- CMIOExtensionStream
-  init(localizedName:streamID:direction:clockType:source:) 

Initializer

# init(localizedName:streamID:direction:clockType:source:)

Creates a stream.

Mac Catalyst 15.4+macOS 12.3+

``` source
init(
    localizedName: String,
    streamID: UUID,
    direction: CMIOExtensionStream.Direction,
    clockType: CMIOExtensionStream.ClockType,
    source: any CMIOExtensionStreamSource
)
```

## Parameters 

`localizedName`  

A localized name for the stream.

`streamID`  

A universally unique identifier for the stream.

`direction`  

The direction of the source, which indicates if it produces or consumes samples.

`clockType`  

A clock type for the stream.

`source`  

The stream source object.

## See Also

### Creating a Stream

init(localizedName: String, streamID: UUID, direction: CMIOExtensionStream.Direction, customClockConfiguration: CMIOExtensionStreamCustomClockConfiguration, source: any CMIOExtensionStreamSource)

Creates a stream that uses a custom clock configuration.

