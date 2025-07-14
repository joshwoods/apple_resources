

- LightweightCodeRequirements
- ValidationCategory
-  ValidationCategory.Value 

Structure

# ValidationCategory.Value

Supported Validation categories for signatures

iOS 17.4+iPadOS 17.4+Mac Catalyst 17.4+macOS 14.4+tvOS 17.4+visionOS 1.1+watchOS 10.4+

``` source
struct Value
```

## Topics

### Initializers

init?(rawValue: Int64)

Creates a new instance with the specified raw value.

### Instance Properties

let rawValue: Int64

The corresponding value of the raw type.

### Type Aliases

typealias RawValue

The raw type that can be used to represent all values of the conforming type.

### Type Properties

static let appStore: ValidationCategory.Value

Indicates that the code is signed by Apple’s App Store

static let developerID: ValidationCategory.Value

Indicates that the code is signed by an Apple issued Developer ID certificate.

static let development: ValidationCategory.Value

Indicates that the code is signed by an Apple issued development certificate.

static let enterprise: ValidationCategory.Value

Indicates that the code is signed by an Apple issued distribution certificate and allowed to run via Provisioning profile.

static let none: ValidationCategory.Value

Indicates that the code is either adhoc signed or signed by an un-recognized certificate chain.

static let platform: ValidationCategory.Value

Indicates that the code is signed by Apple or allowed by a loaded trustcache.

static let testflight: ValidationCategory.Value

Indicates that the code is signed by Apple’s TestFlight certificate

### Default Implementations

Equatable Implementations

RawRepresentable Implementations

## Relationships

### Conforms To

- Copyable
- Decodable
- Encodable
- Equatable
- Hashable
- RawRepresentable
- Sendable

