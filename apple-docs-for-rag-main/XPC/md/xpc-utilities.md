

- XPC
-  Utilities 

API Collection

# Utilities

Browse debugging utilities and constants to use with the XPC APIs.

## Topics

### Debug Functions

func xpc_debugger_api_misuse_info() -> UnsafePointer&lt;CChar>!

Returns a pointer to a string that describes the reason XPC aborts the calling process.

### Version Details

var XPC_API_VERSION: Int32

The version of the XPC API.

var IPHONE_SIMULATOR_HOST_MIN_VERSION_REQUIRED: Int32

The minimum required Simulator host version.

## See Also

### Additional Types

XPC objects

Encapsulate data in objects that represent primitive types, collections, and more.

XPC connections

Create and manage connections to services using connection-based APIs.

