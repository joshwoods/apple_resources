

- ManagedAppDistribution
-  ManagedAppDistributionError 

Enumeration

# ManagedAppDistributionError

Codes that identify errors in Managed App Distribution.

iOS 17.2+iPadOS 17.2+visionOS 2.4+

``` source
enum ManagedAppDistributionError
```

## Topics

### Creating an error object

init(from: any Decoder) throws

Creates a new instance by decoding from the given decoder.

### Inspecting errors

case deviceNotManaged

An error that indicates this device isn’t managed.

case networkError

An error that indicates a network issue.

case unrecoverableError

An error that is unspecified and unrecoverable.

case unsupportedPlatform

An error that indicates the platform is unsupported.

### Providing error information

var description: String

A localized description of the error.

var errorDescription: String?

A brief description of the error.

var failureReason: String?

A detailed description of the error.

var recoveryOptions: [String]

A set of possible recovery options to present.

var recoverySuggestion: String?

A suggestion for recovering from the error.

var localizedStringResource: LocalizedStringResource

A set of localized error strings.

### Providing help information

var helpAnchor: String?

A link to help documentation.

### Recovering from errors

func attemptRecovery(optionIndex: Int) -> Bool

Attempt to recover from this error when someone selects the option at the given index.

func attemptRecovery(optionIndex: Int, resultHandler: (Bool) -> Void)

Attempt to recover from this error when someone selects the option at the given index.

### Operators

static func == (ManagedAppDistributionError, ManagedAppDistributionError) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Enumeration Cases

case appNotManaged

An error that indicates that the calling app is not managed

case licenseNotFound

An error that indicates that a license wasn’t found for requested app.

### Instance Properties

var hashValue: Int

The hash value.

### Instance Methods

func encode(to: any Encoder) throws

Encodes this value into the given encoder.

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

### Default Implementations

Equatable Implementations

Error Implementations

## Relationships

### Conforms To

- Copyable
- CustomLocalizedStringResourceConvertible
- CustomStringConvertible
- Decodable
- Encodable
- Equatable
- Error
- Hashable
- LocalizedError
- RecoverableError
- Sendable

