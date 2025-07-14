

- Virtualization
-  VZLinuxRosettaAvailability 

Enumeration

# VZLinuxRosettaAvailability

Constants that describe the availability and installation status of Rosetta.

macOS 13.0+

``` source
enum VZLinuxRosettaAvailability
```

## Mentioned in 

Running Intel Binaries in Linux VMs with Rosetta

## Topics

### Rosetta availability states

case notSupported

The current hardware or software configuration doesn’t support Rosetta.

case notInstalled

Rosetta isn’t installed.

case installed

Rosetta is available on the host system.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Checking Rosetta availability

class var availability: VZLinuxRosettaAvailability

A value that indicates the current state of Rosetta’s availability.

