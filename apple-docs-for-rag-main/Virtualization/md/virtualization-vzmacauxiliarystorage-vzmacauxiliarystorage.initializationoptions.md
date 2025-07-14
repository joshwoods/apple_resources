

- Virtualization
- VZMacAuxiliaryStorage
-  VZMacAuxiliaryStorage.InitializationOptions 

Structure

# VZMacAuxiliaryStorage.InitializationOptions

Options you can set when creating new auxiliary storage.

macOS 12.0+

``` source
struct InitializationOptions
```

## Topics

### Mac auxiliary storage structure

init(rawValue: UInt)

Creates a new initialization options structure with the value you supply.

### Controlling overwrites

static var allowOverwrite: VZMacAuxiliaryStorage.InitializationOptions

A Boolean value that indicates whether the VM can overwrite an existing auxiliary storage file.

static var allowOverwrite: VZMacAuxiliaryStorage.InitializationOptions

A Boolean value that indicates whether the VM can overwrite an existing auxiliary storage file.

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- ExpressibleByArrayLiteral
- OptionSet
- RawRepresentable
- Sendable
- SetAlgebra

