

- Metal
-  MTLFunctionDescriptor 

Class

# MTLFunctionDescriptor

A description of a function object to create.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
class MTLFunctionDescriptor
```

## Mentioned in 

Compiling Binary Archives from a Custom Configuration Script

## Topics

### Specifying the Function Configuration

var name: String?

The name of the function to fetch from the library.

var specializedName: String?

A new name for the created function object.

var constantValues: MTLFunctionConstantValues?

The set of constant values assigned to the function constants.

var options: MTLFunctionOptions

Flags specifying how Metal should create the new function object.

var binaryArchives: [any MTLBinaryArchive]?

The binary archives to search for a previously-compiled version of this function.

struct MTLFunctionOptions

Options that define how Metal creates the function object.

class MTLLinkedFunctions

A set of related functions that Metal links to when necessary to create the function object.

## Relationships

### Inherits From

- NSObject

### Inherited By

- MTLIntersectionFunctionDescriptor

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCopying
- NSObjectProtocol

## See Also

### Related Documentation

func makeFunction(descriptor: MTLFunctionDescriptor, completionHandler: ((any MTLFunction)?, (any Error)?) -> Void)

Asynchronously creates an object representing a shader function, using the specified descriptor.

**Required**

func makeFunction(descriptor: MTLFunctionDescriptor) throws -> any MTLFunction

Synchronously creates an object representing a shader function, using the specified descriptor.

**Required**

### Shader Functions

protocol MTLFunction

An object that represents a public shader function in a Metal library.

protocol MTLFunctionHandle

An object representing a function that you can add to a visible function table.

class MTLVisibleFunctionTableDescriptor

A specification of how to create a visible function table.

protocol MTLVisibleFunctionTable

A table of shader functions visible to your app that you can pass into compute commands to customize the behavior of a shader.

class MTLIntersectionFunctionDescriptor

A description of an intersection function that performs an intersection test.

class MTLIntersectionFunctionTableDescriptor

A specification of how to create an intersection function table.

protocol MTLIntersectionFunctionTable

A table of intersection functions that Metal calls to perform ray-tracing intersection tests.

