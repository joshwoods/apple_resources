

- AudioDriverKit
- IOUserAudioStream
-  SetTerminalType 

Instance Method

# SetTerminalType

Sets the terminal type of the stream.

DriverKit 21.0+

``` source
kern_return_t SetTerminalType(IOUserAudioStreamTerminalType in_terminal_type);
```

## Parameters 

`in_terminal_type`  

The IOUserAudioStreamTerminalType to set.

## Return Value

kIOReturnSuccess on success, or another value if an error occurs. For a list of error codes, see Error Codes.

## Discussion

If successful, changing the available formats sends a notification to the host to update the object state.

## See Also

### Working with Stream Terminals

GetTerminalType

Gets the terminal type of the stream.

IOUserAudioStreamTerminalType

Constants that describe the terminal type of an audio stream.

