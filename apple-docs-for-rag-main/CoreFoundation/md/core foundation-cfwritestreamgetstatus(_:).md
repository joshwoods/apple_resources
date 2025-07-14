

- Core Foundation
-  CFWriteStreamGetStatus(\_:) 

Function

# CFWriteStreamGetStatus(\_:)

Returns the current state of a stream.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFWriteStreamGetStatus(_ stream: CFWriteStream!) -> CFStreamStatus
```

## Parameters 

`stream`  

The stream to examine.

## Return Value

The current state of `stream`. See CFStreamStatus for the list of possible states.

## See Also

### Examining Stream Properties

func CFWriteStreamCanAcceptBytes(CFWriteStream!) -> Bool

Returns whether a writable stream can accept new data without blocking.

func CFWriteStreamCopyProperty(CFWriteStream!, CFStreamPropertyKey!) -> CFTypeRef!

Returns the value of a property for a stream.

func CFWriteStreamCopyError(CFWriteStream!) -> CFError!

Returns the error associated with a stream.

func CFWriteStreamGetError(CFWriteStream!) -> CFStreamError

Returns the error status of a stream.

Deprecated

