

- Virtualization
- VZEFIVariableStore
-  VZEFIVariableStore.InitializationOptions 

Structure

# VZEFIVariableStore.InitializationOptions

Constants that describe the options available when creating a new Extensible Firmware Interface (EFI) variable store.

macOS 13.0+

``` source
struct InitializationOptions
```

## Topics

### Creating an EFI initialization store

init(rawValue: UInt)

Creates a new EFI variable store with the specified value.

### Constants that control overwriting

static var allowOverwrite: VZEFIVariableStore.InitializationOptions

A Boolean value that indicates whether the framework can overwrite the EFI variable store.

static var allowOverwrite: VZEFIVariableStore.InitializationOptions

A Boolean value that indicates whether the framework can overwrite the EFI variable store.

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

### Creating the variable store

init(creatingVariableStoreAt: URL, options: VZEFIVariableStore.InitializationOptions) throws

Creates a new EFI variable store at specified the URL on the filesystem, initialization options, and error-return variable.

init(url: URL)

Initialize the variable store from the URL of an existing file.

