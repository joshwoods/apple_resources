

- Foundation
- Bundle
-  executableArchitectures 

Instance Property

# executableArchitectures

An array of numbers indicating the architecture types supported by the bundle’s executable.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var executableArchitectures: [NSNumber]? { get }
```

## Discussion

An array of `NSNumber` objects, each of which contains an integer value corresponding to a supported processor architecture. For a list of common architecture types, see the constants in Mach-O Architecture. If the bundle does not contain a Mach-O executable, this is `nil`.

The bundle scans its Mach-O executable and returns all of the architecture types it finds. Because they are taken directly from the executable, the values may not always correspond to one of the well-known CPU types defined in Mach-O Architecture.

## See Also

### Loading Code from a Bundle

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

Mach-O Architecture

Constants that describe the CPU types that a bundle’s executable code supports.

