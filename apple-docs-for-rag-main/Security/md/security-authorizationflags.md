

- Security
-  AuthorizationFlags 

Structure

# AuthorizationFlags

The flags used to specify authorization options.

Mac Catalyst 13.0+macOS 10.0+

``` source
struct AuthorizationFlags
```

## Overview

These flags instruct the Security Server how to proceed with the function in which you pass them. You bitwise `OR` them together to specify more than one at a time. Set all unused bits to `0` to allow for future expansion.

Use these flags in calls to the AuthorizationCreate(_:_:_:_:), AuthorizationFree(_:_:), AuthorizationCopyRights(_:_:_:_:_:), and AuthorizationCopyRightsAsync(_:_:_:_:_:) functions.

## Topics

### Initializers

init(rawValue: UInt32)

Initializes an authorization flags structure.

### Type Properties

static var interactionAllowed: AuthorizationFlags

A flag that permits user interaction as needed.

static var extendRights: AuthorizationFlags

A flag that permits the Security Server to attempt to grant the rights requested.

static var partialRights: AuthorizationFlags

A flag that permits the Security Server to grant rights on an individual basis.

static var destroyRights: AuthorizationFlags

A flag that instructs the Security Server to revoke authorization.

static var preAuthorize: AuthorizationFlags

A flag that instructs the Security Server to preauthorize the rights requested.

static var noData: AuthorizationFlags

Private flag. Do not use.

static var skipInternalAuth: AuthorizationFlags

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- ExpressibleByArrayLiteral
- OptionSet
- RawRepresentable
- Sendable
- SetAlgebra

