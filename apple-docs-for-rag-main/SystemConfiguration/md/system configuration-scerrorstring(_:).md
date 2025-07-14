

- System Configuration
-  SCErrorString(\_:) 

Function

# SCErrorString(\_:)

Returns a string describing the specified status code or error code.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.1+tvOSvisionOS 1.0+

``` source
func SCErrorString(_ status: Int32) -> UnsafePointer
```

## Parameters 

`status`  

A status or error code described in Status and Error Codes. You typically get this code by calling SCError() or SCCopyLastError().

## Return Value

The message string associated with the status or error identified by `status`.

## See Also

### Functions

func SCCopyLastError() -> CFError

Returns an error or status code associated with the most recent function call.

func SCError() -> Int32

Returns an error or status code associated with the most recent function call.

