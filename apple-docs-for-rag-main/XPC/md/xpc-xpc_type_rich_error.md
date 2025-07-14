

- XPC
-  XPC_TYPE_RICH_ERROR 

Global Variable

# XPC_TYPE_RICH_ERROR

A type that represents a rich error object.

iOS 17.0+iPadOS 17.0+Mac CatalystmacOS 14.0+tvOS 17.0+watchOS 10.0+

``` source
var XPC_TYPE_RICH_ERROR: xpc_type_t { get }
```

## See Also

### Errors

struct XPCRichError

An error that contains a description and indicates if you can retry the operation that caused the error.

var XPC_TYPE_ERROR: xpc_type_t

A type that represents an error object.

let XPC_ERROR_KEY_DESCRIPTION: UnsafePointer&lt;CChar>

A key for querying an error dictionary to retrieve a string with a human-readable description of the error.

var XPC_ERROR_PEER_CODE_SIGNING_REQUIREMENT: xpc_object_t

