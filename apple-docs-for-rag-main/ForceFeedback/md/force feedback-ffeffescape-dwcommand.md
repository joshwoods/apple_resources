

- Force Feedback
- FFEFFESCAPE
-  dwCommand 

Instance Property

# dwCommand

Specifies a plugIn specific command number. Contact the hardware vendor for a list of valid commands and their parameters.

Mac Catalyst 13.0+macOS 10.2+

``` source
var dwCommand: DWORD
```

## See Also

### Instance Properties

var cbInBuffer: DWORD

Specifies the size, in bytes, of the **lpvInBuffer** buffer.

var cbOutBuffer: DWORD

On entry, specifies the size, in bytes, of the **lpvOutBuffer** buffer. On exit, specifies the number of bytes actually produced by the command.

var dwSize: DWORD

Size, in bytes, of this structure. This member must be initialized before the structure is used.

var lpvInBuffer: UnsafeMutableRawPointer!

Buffer containing the data required to perform the operation.

var lpvOutBuffer: UnsafeMutableRawPointer!

Buffer in which the operation’s output data is returned.

