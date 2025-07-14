

- Security
-  SessionCreationFlags 

Structure

# SessionCreationFlags

The flags that affect the creation of a security session.

Mac Catalyst 13.0+macOS 10.0+

``` source
struct SessionCreationFlags
```

## Topics

### Initializers

init(rawValue: UInt32)

Initializes a session creation flags value.

### Flags

static var sessionKeepCurrentBootstrap: SessionCreationFlags

The caller has allocated sub-bootstrap.

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- ExpressibleByArrayLiteral
- OptionSet
- RawRepresentable
- Sendable
- SetAlgebra

