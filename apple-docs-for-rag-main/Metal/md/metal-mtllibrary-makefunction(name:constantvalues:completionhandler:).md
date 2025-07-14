

- Metal
- MTLLibrary
-  makeFunction(name:constantValues:completionHandler:) 

Instance Method

# makeFunction(name:constantValues:completionHandler:)

Asynchronously creates a specialized shader function.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+

``` source
func makeFunction(
    name: String,
    constantValues: MTLFunctionConstantValues,
    completionHandler: @escaping ((any MTLFunction)?, (any Error)?) -> Void
)
```

``` source
func makeFunction(
    name: String,
    constantValues: MTLFunctionConstantValues
) async throws -> any MTLFunction
```

**Required**

## Parameters 

`name`  

The name of the specialized function.

`constantValues`  

The set of constant values assigned to the function constants. Compilation fails if you don’t provide valid constant values for all required function constants.

`completionHandler`  

A block of code that Metal calls after it creates the specialized function.

function  
A specialized function, or `nil` if an error occurred.

error  
An error object that describes compilation problems, if any. This object contains compiler errors if the specialized function is `nil`, and compiler warnings if Metal created the specialized function with warnings. If Metal created the function without errors or warnings, this error object is `nil`.

## Discussion

Function constant values are first looked up by their index, then by their name. Metal ignores any values that don’t correspond to a function constant in the named function without generating errors or warnings.

## See Also

### Creating Shader Function Objects

func makeFunction(name: String) -> (any MTLFunction)?

Creates an object that represents a shader function in the library.

**Required**

func makeFunction(name: String, constantValues: MTLFunctionConstantValues) throws -> any MTLFunction

Synchronously creates a specialized shader function.

**Required**

func makeFunction(descriptor: MTLFunctionDescriptor, completionHandler: ((any MTLFunction)?, (any Error)?) -> Void)

Asynchronously creates an object representing a shader function, using the specified descriptor.

**Required**

func makeFunction(descriptor: MTLFunctionDescriptor) throws -> any MTLFunction

Synchronously creates an object representing a shader function, using the specified descriptor.

**Required**

