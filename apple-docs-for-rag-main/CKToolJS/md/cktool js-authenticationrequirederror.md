

- CKTool JS
-  AuthenticationRequiredError 

Structure

# AuthenticationRequiredError

An object that represents an error that occurs when authentication information is missing for the current user.

CKTool JS 1.2.15+

``` source
dictionary AuthenticationRequiredError {
 Int32 code;
 string message;
 string reason;
 string? detailedMessage;
 string? requestUuid;
 Int32? retryAfterSeconds;
 string redirectUrl;
};
```

## Overview

Some database operations require that users sign in with their Apple ID. The server returns `AuthenticationRequiredError` when the user isn’t signed in or their session has expired.

In JavaScript, this is a plain object with properties as described.

In TypeScript, this type is imported in the following way:

```
import type { AuthenticationRequiredError } from "@apple/cktool.database";
```

## Topics

### Instance Properties

code

The HTTP status code for a request error.

detailedMessage

A string that contains any additional information about this error.

message

A string containing the code for the error that occurred.

reason

A string that indicates the reason for the error.

redirectUrl

A redirect URL for the user to securely sign in using their Apple ID.

requestUuid

A unique identifier for this error.

retryAfterSeconds

The suggested time to wait in seconds before trying this operation again.

## See Also

### Database Errors

CKDBBatchDeleteError

An object that represents an error that may occur when deleting a resource as part of a batch delete operation.

RequestError

An object that represents a general error from the service.

