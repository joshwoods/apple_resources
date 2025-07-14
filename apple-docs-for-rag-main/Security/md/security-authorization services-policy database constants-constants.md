

- Security
- Authorization Services
-  Policy Database Constants 

API Collection

# Policy Database Constants

Use these constants to set rights and rules in the policy database.

## Overview

Use these constants when creating or modifying a rule in the policy database using the AuthorizationRightSet(_:_:_:_:_:_:) function.

## Topics

### Constants

var kAuthorizationRightRule: String

Indicates a rule delegation key.

var kAuthorizationRuleIsAdmin: String

Indicates a delegate rule definition constant specifying that the user must be an administrator.

var kAuthorizationRuleAuthenticateAsAdmin: String

Indicates a delegate rule definition constant specifying that the user must authenticate as an administrator.

var kAuthorizationRuleAuthenticateAsSessionUser: String

Indicates a delegate rule definition constant specifying that the user must authenticate as the session owner (logged-in user).

var kAuthorizationRuleClassAllow: String

Indicates a delegate rule definition constant that always allows the specified right.

var kAuthorizationRuleClassDeny: String

Indicates a delegate rule definition constant that always denies the specified right.

var kAuthorizationComment: String

Indicates comments for a rule.

