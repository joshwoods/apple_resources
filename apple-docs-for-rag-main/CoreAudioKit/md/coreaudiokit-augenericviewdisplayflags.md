

- CoreAudioKit
-  AUGenericViewDisplayFlags 

Structure

# AUGenericViewDisplayFlags

Flags that describe the display of a generic view.

macOS

``` source
struct AUGenericViewDisplayFlags
```

## Topics

### Display Flags

static var viewParametersDisplayFlag: AUGenericViewDisplayFlags

If set, the generic view displays the audio unit parameters of the audio unit.

static var viewPropertiesDisplayFlag: AUGenericViewDisplayFlags

If set, the generic view displays the audio unit properties of the audio unit.

static var viewTitleDisplayFlag: AUGenericViewDisplayFlags

If set, the generic view displays the title and manufacturer of the audio unit.

### Initializers

init(rawValue: UInt32)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- ExpressibleByArrayLiteral
- OptionSet
- RawRepresentable
- Sendable
- SetAlgebra

