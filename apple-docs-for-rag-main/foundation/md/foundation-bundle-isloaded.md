

- Foundation
- Bundle
-  isLoaded 

Instance Property

# isLoaded

The load status of a bundle.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var isLoaded: Bool { get }
```

## Discussion

true if the bundle’s code is currently loaded, otherwise false.

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

Mach-O Architecture

Constants that describe the CPU types that a bundle’s executable code supports.

