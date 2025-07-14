

- CKTool JS
-  CKDBBatchDeleteError 

Structure

# CKDBBatchDeleteError

An object that represents an error that may occur when deleting a resource as part of a batch delete operation.

CKTool JS 1.2.15+

``` source
dictionary CKDBBatchDeleteError {
 string id;
 string code;
 string message;
};
```

## Overview

In JavaScript, this is a plain object with properties as described.

In TypeScript, this type is imported in the following way:

```
import type { CKDBBatchDeleteError } from "@apple/cktool.database";
```

## Topics

### Instance Properties

code

A string that contains the code for the error that occurred.

id

The identifier for the resource that failed to be deleted.

message

A string that indicates the reason for the error.

## See Also

### Database Errors

AuthenticationRequiredError

An object that represents an error that occurs when authentication information is missing for the current user.

RequestError

An object that represents a general error from the service.

