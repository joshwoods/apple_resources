

- Core Foundation
-  CFWriteStreamCanAcceptBytes(\_:) 

Function

# CFWriteStreamCanAcceptBytes(\_:)

Returns whether a writable stream can accept new data without blocking.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFWriteStreamCanAcceptBytes(_ stream: CFWriteStream!) -> Bool
```

## Parameters 

`stream`  

The stream to examine.

## Return Value

`true` if data can be written to `stream` without blocking, `false` otherwise. If `stream` cannot tell if data can be written without actually trying to write the data, this function returns `true`.

## See Also

### Examining Stream Properties

func CFWriteStreamCopyProperty(CFWriteStream!, CFStreamPropertyKey!) -> CFTypeRef!

Returns the value of a property for a stream.

func CFWriteStreamCopyError(CFWriteStream!) -> CFError!

Returns the error associated with a stream.

func CFWriteStreamGetError(CFWriteStream!) -> CFStreamError

Returns the error status of a stream.

Deprecated

func CFWriteStreamGetStatus(CFWriteStream!) -> CFStreamStatus

Returns the current state of a stream.

