

- Security Interface
-  SFViewType 

Structure

# SFViewType

These constants define the view type requested by the authorization plug-in.

macOS 10.3+

``` source
struct SFViewType
```

## Topics

### Initializers

init(UInt32)

init(rawValue: UInt32)

### Instance Properties

var rawValue: UInt32

### Constants

var SFViewTypeIdentityAndCredentials: SFViewType

Indicates a view that contains controls for identity and credentials was requested by the authorization plug-in.

var SFViewTypeCredentials: SFViewType

Indicates a view that contains controls for credentials was requested by the authorization plug-in.

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Reference

struct SFAuthorizationViewState

Defines the current state of the authorization view.

struct SFButtonType

These constants define the button types used by authorization plug-ins.

SecurityInterface Constants

Constants in the SecurityInterface framework.

SecurityInterface Data Types

Data types found in the Security Interface framework.

SecurityInterface Enumerations

