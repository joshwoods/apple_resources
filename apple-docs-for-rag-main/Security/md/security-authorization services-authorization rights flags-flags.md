

- Security
- Authorization Services
-  Authorization Rights Flags 

API Collection

# Authorization Rights Flags

Recognize the values the Security Server sets in an authorization item’s flag field.

## Overview

Look for these values in the flags field of an AuthorizationItem, for example among the set of items in the `authorizedRights` parameter returned by a call to the AuthorizationCopyInfo(_:_:_:) function.

## Topics

### Constants

var kAuthorizationFlagCanNotPreAuthorize: Int

Indicates the Security Server could not preauthorizethe right.

