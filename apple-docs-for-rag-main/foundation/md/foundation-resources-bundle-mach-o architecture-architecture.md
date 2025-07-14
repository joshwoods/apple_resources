

- Foundation
- Resources
- Bundle
-  Mach-O Architecture 

API Collection

# Mach-O Architecture

Constants that describe the CPU types that a bundle’s executable code supports.

## Topics

### Constants

var NSBundleExecutableArchitectureARM64: Int

The 64-bit ARM architecture.

var NSBundleExecutableArchitectureI386: Int

The 32-bit Intel architecture.

var NSBundleExecutableArchitectureX86_64: Int

The 64-bit Intel architecture.

var NSBundleExecutableArchitecturePPC: Int

The 32-bit PowerPC architecture.

var NSBundleExecutableArchitecturePPC64: Int

The 64-bit PowerPC architecture.

## See Also

### Loading Code from a Bundle

var executableArchitectures: [NSNumber]?

An array of numbers indicating the architecture types supported by the bundle’s executable.

func preflight() throws

Returns a Boolean value indicating whether the bundle’s executable code could be loaded successfully.

func load() -> Bool

Dynamically loads the bundle’s executable code into a running program, if the code has not already been loaded.

func loadAndReturnError() throws

Loads the bundle’s executable code and returns any errors.

func unload() -> Bool

Unloads the code associated with the receiver.

var isLoaded: Bool

The load status of a bundle.

