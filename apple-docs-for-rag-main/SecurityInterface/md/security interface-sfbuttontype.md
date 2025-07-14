

- Security Interface
-  SFButtonType 

Structure

# SFButtonType

These constants define the button types used by authorization plug-ins.

macOS 10.3+

``` source
struct SFButtonType
```

## Topics

### Initializers

init(UInt32)

init(rawValue: UInt32)

### Instance Properties

var rawValue: UInt32

### Constants

var SFButtonTypeCancel: SFButtonType

Indicates the Cancel button was pressed.

var SFButtonTypeOK: SFButtonType

Indicates the OK button was pressed.

var SFButtonTypeBack: SFButtonType

Indicates the Back button was pressed.

var SFButtonTypeLogin: SFButtonType

Indicates the Login button was pressed.

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

struct SFViewType

These constants define the view type requested by the authorization plug-in.

SecurityInterface Constants

Constants in the SecurityInterface framework.

SecurityInterface Data Types

Data types found in the Security Interface framework.

SecurityInterface Enumerations

