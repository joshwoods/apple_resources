

- Security
-  SessionAttributeBits 

Structure

# SessionAttributeBits

The attributes of a security session.

Mac Catalyst 13.0+macOS 10.0+

``` source
struct SessionAttributeBits
```

## Topics

### Initializers

init(rawValue: UInt32)

Initializes a session attribute bits structure.

### Bits

static var sessionIsRoot: SessionAttributeBits

A bit that indicates the session is the root session.

static var sessionHasGraphicAccess: SessionAttributeBits

A bit that indicates a graphic subsystem is available.

static var sessionHasTTY: SessionAttributeBits

A bit that indicates `/dev/tty` is available.

static var sessionIsRemote: SessionAttributeBits

A bit that indicates the session was initiated over the network.

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- ExpressibleByArrayLiteral
- OptionSet
- RawRepresentable
- Sendable
- SetAlgebra

