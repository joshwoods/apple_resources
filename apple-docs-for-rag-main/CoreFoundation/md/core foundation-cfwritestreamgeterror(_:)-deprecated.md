

- Core Foundation
-  CFWriteStreamGetError(\_:) Deprecated

Function

# CFWriteStreamGetError(\_:)

Returns the error status of a stream.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFWriteStreamGetError(_ stream: CFWriteStream!) -> CFStreamError
```

Deprecated

Use CFWriteStreamCopyError(_:) instead.

## Parameters 

`stream`  

The stream to examine.

## Return Value

The error status of `stream` returned in a CFStreamError structure.

## See Also

### Examining Stream Properties

func CFWriteStreamCanAcceptBytes(CFWriteStream!) -> Bool

Returns whether a writable stream can accept new data without blocking.

func CFWriteStreamCopyProperty(CFWriteStream!, CFStreamPropertyKey!) -> CFTypeRef!

Returns the value of a property for a stream.

func CFWriteStreamCopyError(CFWriteStream!) -> CFError!

Returns the error associated with a stream.

func CFWriteStreamGetStatus(CFWriteStream!) -> CFStreamStatus

Returns the current state of a stream.

