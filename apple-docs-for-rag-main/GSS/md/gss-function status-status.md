

- GSS
-  Function Status 

API Collection

# Function Status

Evaluate return values that most GSS-API functions use to indicate the outcome of an operation.

## Overview

The functions of the GSS-API return two status codes. The major status code, delivered as the function’s return value, provides a mechanism-independent status output. A value of GSS_S_COMPLETE typically indicates success, but the code is actually composed of several fields that enable communicating a more nuanced result. Always check the major status code to determine if an operation succeeds.

The minor status code provides additional information, often mechanism-specific, when an operation fails. This result returns using the OM_uint32 pointer given as the function’s first argument. Examine this value to further debug a problem. For example, many functions allocate memory as a side effect of their main task. If memory allocation fails, the entire operation fails. But while the major status indicates a generic problem, a minor status of `ENOMEM` indicates that failed memory allocation is the exact culprit.

Three bitfields bundled together make up major status codes in a single OM_uint32 value. These fields are:

The calling error  
A generic GSS-API error in the most significant 8 bits.

The routine error  
An error specific to the routine in the next 8 bits.

Supplementary Information  
Additional information about the error in the lower 16 bits.

When a function successfully runs to completion, it returns zero for all of these fields. As a convenience, you can compare the result directly with the status code GSS_S_COMPLETE to test for this condition.

For any other result, use one of the available extraction macros (such as GSS_CALLING_ERROR) to obtain a value that you compare against one of the known error codes. For example, you can test for a failure to read one of the function inputs as follows:

```
OM_uint32 major = 
if (GSS_CALLING_ERROR(major) == GSS_S_CALL_INACCESSIBLE_READ) {
    // Handle the error
}
```

Use the gss_display_status(_:_:_:_:_:_:) function to retrieve a human readable string corresponding to a given status result.

## Topics

### Status and Error Creation

typealias OM_uint32

A 32-bit unsigned integer.

typealias OM_uint64

A 64-bit unsigned integer.

typealias gss_uint32

A 32-bit unsigned integer.

typealias gss_status_id_t

A pointer to a status result.

var GSS_C_MECH_CODE: Int32

A flag that indicates the status code comes from a call to an underlying mechanism, such as Kerberos.

var GSS_C_GSS_CODE: Int32

A flag that indicates the named status code comes from a GSS-API call.

var GSS_S_COMPLETE: Int32

The operation completed without error.

func gss_display_status(UnsafeMutablePointer&lt;OM_uint32>, OM_uint32, Int32, gss_OID?, UnsafeMutablePointer&lt;OM_uint32>, gss_buffer_t) -> OM_uint32

Returns a human readable string for a status code.

func GSSCreateError(gss_const_OID, OM_uint32, OM_uint32) -> Unmanaged&lt;CFError>?

Returns an error object based on GSS-API major and minor status codes.

### Calling Errors

var GSS_S_CALL_BAD_STRUCTURE: UInt

Improperly formatted parameter.

var GSS_S_CALL_INACCESSIBLE_READ: UInt

A required input parameter could not be read.

var GSS_S_CALL_INACCESSIBLE_WRITE: UInt

A required output parameter failed to write.

### Routine Errors

var GSS_S_BAD_MECH: UInt

Unsupported mechanism.

var GSS_S_BAD_NAME: UInt

Invalid name.

var GSS_S_BAD_NAMETYPE: UInt

Unsupported name type.

var GSS_S_BAD_MIC: UInt

Failed token integrity check.

var GSS_S_BAD_SIG: UInt

Failed token integrity check.

var GSS_S_BAD_STATUS: UInt

Invalid status selector.

var GSS_S_BAD_BINDINGS: UInt

Channel bindings mismatch.

var GSS_S_NO_CRED: UInt

No valid credentials.

var GSS_S_NO_CONTEXT: UInt

No valid security context.

var GSS_S_DEFECTIVE_TOKEN: UInt

Defective token.

var GSS_S_DEFECTIVE_CREDENTIAL: UInt

Defective credential.

var GSS_S_CREDENTIALS_EXPIRED: UInt

Expired credential.

var GSS_S_CONTEXT_EXPIRED: UInt

Expired context.

var GSS_S_FAILURE: UInt

An unspecified error.

var GSS_S_BAD_QOP: UInt

Unsupported QOP value.

var GSS_S_UNAUTHORIZED: UInt

Unauthorized operation.

var GSS_S_UNAVAILABLE: UInt

Unavailable operation.

var GSS_S_DUPLICATE_ELEMENT: UInt

A duplicate credential element requested.

var GSS_S_NAME_NOT_MN: UInt

The name contains multimechanism elements.

var GSS_S_BAD_MECH_ATTR: UInt

Unknown mechanism attribute.

var GSS_S_CRED_UNAVAIL: UInt

Unavailable credential.

### Masks and Offsets

var GSS_C_CALLING_ERROR_MASK: UInt

A mask with a width that matches the calling error field.

var GSS_C_CALLING_ERROR_OFFSET: Int32

The offset of the calling error field within the major status code.

var GSS_C_ROUTINE_ERROR_MASK: UInt

A mask with a width that matches the routine error field.

var GSS_C_ROUTINE_ERROR_OFFSET: Int32

The offset of the routine error field within the major status code.

var GSS_C_SUPPLEMENTARY_MASK: UInt

A mask with a width that matches the supplementary information field.

var GSS_C_SUPPLEMENTARY_OFFSET: Int32

The offset of the supplementary information field within the major status code.

## See Also

### Memory and Context

Allocating and Releasing Objects

Manage memory and object lifetimes.

Buffer Management

Allocate and deallocate buffers with structures that hold a variety of data.

Context Services

Use context services to manage secure operations between endpoints.

