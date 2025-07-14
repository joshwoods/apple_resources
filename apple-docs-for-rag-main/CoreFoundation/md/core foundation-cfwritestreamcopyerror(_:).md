

- Core Foundation
-  CFWriteStreamCopyError(\_:) 

Function

# CFWriteStreamCopyError(\_:)

Returns the error associated with a stream.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func CFWriteStreamCopyError(_ stream: CFWriteStream!) -> CFError!
```

## Parameters 

`stream`  

The stream to examine.

## Return Value

A CFError object that describes the current problem with stream, or `NULL` if there is no error. Ownership follows the The Create Rule.

## See Also

### Examining Stream Properties

func CFWriteStreamCanAcceptBytes(CFWriteStream!) -> Bool

Returns whether a writable stream can accept new data without blocking.

func CFWriteStreamCopyProperty(CFWriteStream!, CFStreamPropertyKey!) -> CFTypeRef!

Returns the value of a property for a stream.

func CFWriteStreamGetError(CFWriteStream!) -> CFStreamError

Returns the error status of a stream.

Deprecated

func CFWriteStreamGetStatus(CFWriteStream!) -> CFStreamStatus

Returns the current state of a stream.

