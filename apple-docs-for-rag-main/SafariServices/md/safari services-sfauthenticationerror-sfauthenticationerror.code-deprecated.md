

- Safari Services
- SFAuthenticationError
-  SFAuthenticationError.Code Deprecated

Enumeration

# SFAuthenticationError.Code

Messages that describe an authentication error.

iOS 11.0–12.0DeprecatediPadOS 11.0–12.0DeprecatedMac Catalyst 13.1–13.1Deprecated

**Mac Catalyst**

``` source
enum SFAuthenticationError
```

**iOS, iPadOS**

``` source
enum Code
```

Deprecated

Use ASWebAuthenticationSessionError.Code instead.

## Topics

### Enumeration Cases

case canceledLogin

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
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

struct SFAuthenticationError

An authentication error.

Deprecated

let SFAuthenticationErrorDomain: String

The domain for authentication errors.

Deprecated

