

- File Provider
- NSFileProviderDomain
-  NSFileProviderDomain.TestingModes 

Structure

# NSFileProviderDomain.TestingModes

Modes that modify the system’s behavior while testing.

iOS 16.0+iPadOS 16.0+macOS 11.3+visionOS 1.0+

``` source
struct TestingModes
```

## Topics

### Accessing Modes

static var alwaysEnabled: NSFileProviderDomain.TestingModes

A testing mode that automatically enables the domain.

static var interactive: NSFileProviderDomain.TestingModes

A testing mode where the extension can deterministically test asynchronous operations.

### Creating Modes

init(rawValue: UInt)

Returns a newly-created testing mode.

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

### Testing

var testingModes: NSFileProviderDomain.TestingModes

A mode that gives the File Provider extension more control over the system’s behavior during testing.

