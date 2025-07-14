

- Safari Services
-  SFAuthenticationError Deprecated

Structure

# SFAuthenticationError

An authentication error.

iOS 11.0–12.0DeprecatediPadOS 11.0–12.0Deprecated

``` source
struct SFAuthenticationError
```

Deprecated

Use ASWebAuthenticationSessionError instead.

## Topics

### Type Properties

static var canceledLogin: SFAuthenticationError.Code

static var errorDomain: String

### Enumerations

enum Code

Messages that describe an authentication error.

## Relationships

### Conforms To

- CustomNSError
- Equatable
- Error
- Hashable
- Sendable

## See Also

### Deprecated

let SFContentBlockerErrorDomain: String

The domain for content blocker errors.

Deprecated

enum SFContentBlockerErrorCode

Messages that describe a content blocker error.

Deprecated

class SFAuthenticationSession

A class that manages sharing a one-time login between Safari and an app, which can also provide automatic login for associated apps.

Deprecated

enum Code

Messages that describe an authentication error.

Deprecated

let SFAuthenticationErrorDomain: String

The domain for authentication errors.

Deprecated

