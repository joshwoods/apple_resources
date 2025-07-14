

- Security
- Sessions
-  Sessions API Result Codes 

API Collection

# Sessions API Result Codes

Recognize result codes specific to the sessions API.

## Discussion

Use the SecCopyErrorMessageString(_:_:) function to obtain a human readable string corresponding to these status codes.

The functions of the sessions API may also return result codes from the authorization services API listed in Authorization Services Result Codes or the general codes listed in Security Framework Result Codes.

## Topics

### Codes

var errSessionSuccess: OSStatus

The operation completed successfully.

var errSessionInvalidId: OSStatus

Detected an invalid session ID.

var errSessionInvalidAttributes: OSStatus

Detected an invalid set of request attribute bits.

var errSessionAuthorizationDenied: OSStatus

Authorization denied.

var errSessionValueNotSet: OSStatus

The requested session attribute has not been set.

var errSessionInternal: OSStatus

An unrecognized internal error occurred.

var errSessionInvalidFlags: OSStatus

Encountered invalid flags or options.

