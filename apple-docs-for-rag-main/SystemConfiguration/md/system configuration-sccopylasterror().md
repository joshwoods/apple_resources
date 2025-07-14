

- System Configuration
-  SCCopyLastError() 

Function

# SCCopyLastError()

Returns an error or status code associated with the most recent function call.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOSvisionOS 1.0+

``` source
func SCCopyLastError() -> CFError
```

## Return Value

The most recent status or error code generated as the result of calling a function defined by the System Configuration framework. The code is represented by a Core Foundation `CFErrorRef` opaque type.

## Discussion

Call the CFErrorGetCode(_:) function on the returned object to get the underlying error-code integer. See Status and Error Codes for descriptions of these codes. For more on `CFErrorRef` objects, see doc://com.apple.documentation/documentation/corefoundation/cferror-ru8.

## See Also

### Functions

func SCError() -> Int32

Returns an error or status code associated with the most recent function call.

func SCErrorString(Int32) -> UnsafePointer&lt;CChar>

Returns a string describing the specified status code or error code.

