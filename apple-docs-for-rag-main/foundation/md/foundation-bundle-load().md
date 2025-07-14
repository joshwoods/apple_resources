

- Foundation
- Bundle
-  load() 

Instance Method

# load()

Dynamically loads the bundle’s executable code into a running program, if the code has not already been loaded.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func load() -> Bool
```

## Return Value

true if the method successfully loads the bundle’s code or if the code has already been loaded, otherwise false.

## Discussion

You can use this method to load the code associated with a dynamically loaded bundle, such as a plug-in or framework. Prior to OS X version 10.5, a bundle would attempt to load its code—if it had any—only once. Once loaded, you could not unload that code. In macOS 10.5 and later, you can unload a bundle’s executable code using the unload() method.

You don’t need to load a bundle’s executable code to search the bundle’s resources.

This method initializes the principal class in the bundle. To add code you want executed after loading, override the initialize() class method of the principal class.

### Special Considerations

If an `NSBundle` object calls the load() method, it calls the unload() method before being deallocated. Therefore, you should retain any `NSBundle` object for as long as any code from it is used by the app.

## See Also

### Related Documentation

var principalClass: AnyClass?

The bundle’s principal class.

func classNamed(String) -> AnyClass?

Returns the `Class` object for the specified name.

### Loading Code from a Bundle

var executableArchitectures: [NSNumber]?

An array of numbers indicating the architecture types supported by the bundle’s executable.

func preflight() throws

Returns a Boolean value indicating whether the bundle’s executable code could be loaded successfully.

func loadAndReturnError() throws

Loads the bundle’s executable code and returns any errors.

func unload() -> Bool

Unloads the code associated with the receiver.

var isLoaded: Bool

The load status of a bundle.

Mach-O Architecture

Constants that describe the CPU types that a bundle’s executable code supports.

