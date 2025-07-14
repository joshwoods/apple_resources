

- Core Media I/O
- CMIOExtensionStream
- CMIOExtensionStream.ClockType
-  CMIOExtensionStream.ClockType.custom 

Case

# CMIOExtensionStream.ClockType.custom

Indicates that the stream’s clock is specific to the device hosting the stream.

Mac Catalyst 15.4+macOS 12.3+

``` source
case custom
```

## Discussion

The extension doesn’t set this type directly. Instead, the system sets it automatically when you specify a CMIOExtensionStreamCustomClockConfiguration when you create a CMIOExtensionStream.

## See Also

### Clock Types

case hostTime

Indicates that the stream uses the host time clock.

case linkedCoreAudioDeviceUID

Indicates that the stream uses the clock of the linked Core Audio device.

