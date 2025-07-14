

- Security
- Authorization Services
-  Authorization Services Result Codes 

API Collection

# Authorization Services Result Codes

Recognize result codes specific to the authorization services API.

## Overview

Use the SecCopyErrorMessageString(_:_:) function to obtain a human readable string corresponding to these status codes.

The functions of the Authorization Services API may also return the general codes listed in Security Framework Result Codes.

## Topics

### Codes

var errAuthorizationSuccess: OSStatus

The operation completed successfully.

var errAuthorizationInvalidSet: OSStatus

The set parameter is invalid.

var errAuthorizationInvalidRef: OSStatus

The authorization parameter is invalid.

var errAuthorizationInvalidTag: OSStatus

The tag parameter is invalid.

var errAuthorizationInvalidPointer: OSStatus

The authorizedRights parameter is invalid.

var errAuthorizationDenied: OSStatus

The Security Server denied authorization for one or more requested rights.

var errAuthorizationCanceled: OSStatus

The user canceled the operation.

var errAuthorizationInteractionNotAllowed: OSStatus

The Security Server denied authorization because no user interaction is allowed.

var errAuthorizationInternal: OSStatus

An unrecognized internal error occurred.

var errAuthorizationExternalizeNotAllowed: OSStatus

The Security Server denied externalization of the authorization reference.

var errAuthorizationInternalizeNotAllowed: OSStatus

The Security Server denied internalization of the authorization reference.

var errAuthorizationInvalidFlags: OSStatus

The flags parameter is invalid.

var errAuthorizationToolExecuteFailure: OSStatus

The tool failed to execute.

var errAuthorizationToolEnvironmentError: OSStatus

The attempt to execute the tool failed to return a success or an error code.

var errAuthorizationBadAddress: OSStatus

The requested socket address is invalid.

