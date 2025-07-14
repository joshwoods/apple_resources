

- AudioDriverKit
- IOUserAudioStream
-  GetTerminalType 

Instance Method

# GetTerminalType

Gets the terminal type of the stream.

DriverKit 21.0+

``` source
IOUserAudioStreamTerminalType GetTerminalType();
```

## Return Value

The stream’s terminal type.

## Discussion

This method synchronizes by using the work queue created by the object.

## See Also

### Working with Stream Terminals

SetTerminalType

Sets the terminal type of the stream.

IOUserAudioStreamTerminalType

Constants that describe the terminal type of an audio stream.

