

- Metal
- MTLLibrary
-  makeFunction(name:constantValues:) 

Instance Method

# makeFunction(name:constantValues:)

Synchronously creates a specialized shader function.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+

``` source
func makeFunction(
    name: String,
    constantValues: MTLFunctionConstantValues
) throws -> any MTLFunction
```

**Required**

## Parameters 

`name`  

The name of the specialized function.

`constantValues`  

The set of constant values assigned to the function constants. Compilation fails if you do not provide valid constant values for all required function constants.

## Return Value

A new MTLFunction instance if the method completes successfully; otherwise Swift throws an error and Objective-C returns `nil`.

## Discussion

Function constant values are first looked up by their index, then by their name. Any values that do not correspond to a function constant in the named function are ignored (without generating errors or warnings).

## See Also

### Creating Shader Function Objects

func makeFunction(name: String) -> (any MTLFunction)?

Creates an object that represents a shader function in the library.

**Required**

func makeFunction(name: String, constantValues: MTLFunctionConstantValues, completionHandler: ((any MTLFunction)?, (any Error)?) -> Void)

Asynchronously creates a specialized shader function.

**Required**

func makeFunction(descriptor: MTLFunctionDescriptor, completionHandler: ((any MTLFunction)?, (any Error)?) -> Void)

Asynchronously creates an object representing a shader function, using the specified descriptor.

**Required**

func makeFunction(descriptor: MTLFunctionDescriptor) throws -> any MTLFunction

Synchronously creates an object representing a shader function, using the specified descriptor.

**Required**

