

- ProximityReader
- VASReadResult
- VASReadResult.ReadEntry
-  VASReadResult.ReadEntry.Status 

Enumeration

# VASReadResult.ReadEntry.Status

Status words that indicate the possible read outcomes.

iOS 15.4+iPadOS 15.4+Mac Catalyst 17.0+

``` source
enum Status
```

## Topics

### Getting the status

case success

case incorrectData

case unsupportedApplicationVersion

case userInterventionRequired

case vasDataNotActivated

case vasDataNotFound

case wrongCommandLength

case wrongP1P2

### Initializers

init?(rawValue: Int)

Creates a new instance with the specified raw value.

### Instance Properties

var rawValue: Int

The corresponding value of the raw type.

### Type Aliases

typealias RawValue

The raw type that can be used to represent all values of the conforming type.

### Default Implementations

Equatable Implementations

RawRepresentable Implementations

## Relationships

### Conforms To

- Copyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Getting the status word

let status: VASReadResult.ReadEntry.Status

The status word that represents the outcome of the VAS read attempt for this reward pass.

