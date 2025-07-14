

- Core Foundation
-  CFStringNormalizationForm 

Enumeration

# CFStringNormalizationForm

Unicode normalization forms as described in Unicode Technical Report \#15.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
enum CFStringNormalizationForm
```

## Topics

### Constants

case D

Canonical decomposition.

case KD

Compatibility decomposition.

case C

Canonical decomposition followed by canonical composition.

case KC

Compatibility decomposition followed by canonical composition.

### Initializers

init?(rawValue: CFIndex)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Constants

Transform Identifiers for CFStringTransform

Constants that identify transforms used with CFStringTransform(_:_:_:_:).

