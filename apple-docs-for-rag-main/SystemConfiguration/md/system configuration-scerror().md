

- System Configuration
-  SCError() 

Function

# SCError()

Returns an error or status code associated with the most recent function call.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.1+tvOSvisionOS 1.0+

``` source
func SCError() -> Int32
```

## Return Value

The most recent status or error code generated as the result of calling a function defined by the System Configuration framework. See Status and Error Codes for descriptions of these codes.

## See Also

### Functions

func SCCopyLastError() -> CFError

Returns an error or status code associated with the most recent function call.

func SCErrorString(Int32) -> UnsafePointer&lt;CChar>

Returns a string describing the specified status code or error code.

