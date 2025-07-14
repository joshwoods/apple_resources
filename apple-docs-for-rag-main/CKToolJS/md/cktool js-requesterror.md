

- CKTool JS
-  RequestError 

Structure

# RequestError

An object that represents a general error from the service.

CKTool JS 1.2.15+

``` source
dictionary RequestError {
 Int32 code;
 string message;
 string reason;
 string? detailedMessage;
 string? requestUuid;
 Int32? retryAfterSeconds;
};
```

## Overview

In JavaScript, this is a plain object with properties as described.

In TypeScript, this type is imported in the following way:

```
import type { RequestError } from "@apple/cktool.database";
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

requestUuid

A unique identifier for this error.

retryAfterSeconds

The suggested time to wait in seconds before trying this operation again.

## See Also

### Database Errors

AuthenticationRequiredError

An object that represents an error that occurs when authentication information is missing for the current user.

CKDBBatchDeleteError

An object that represents an error that may occur when deleting a resource as part of a batch delete operation.

