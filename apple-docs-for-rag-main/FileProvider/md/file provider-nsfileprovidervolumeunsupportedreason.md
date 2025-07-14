

- File Provider
-  NSFileProviderVolumeUnsupportedReason 

Structure

# NSFileProviderVolumeUnsupportedReason

Constants that describe why an external volume might not be eligible for storing a domain.

macOS 15.0+

``` source
struct NSFileProviderVolumeUnsupportedReason
```

## Topics

### Reasons

static var unknown: NSFileProviderVolumeUnsupportedReason

static var nonEncrypted: NSFileProviderVolumeUnsupportedReason

static var readOnly: NSFileProviderVolumeUnsupportedReason

static var network: NSFileProviderVolumeUnsupportedReason

static var quarantined: NSFileProviderVolumeUnsupportedReason

### Initializers

init(rawValue: UInt)

### Type Properties

static var nonAPFS: NSFileProviderVolumeUnsupportedReason

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- ExpressibleByArrayLiteral
- OptionSet
- RawRepresentable
- Sendable
- SetAlgebra

## See Also

### Determining eligibility

case eligible

case ineligible(NSFileProviderVolumeUnsupportedReason)

