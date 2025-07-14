

- Metal
- MTLLibrary
-  makeFunction(descriptor:completionHandler:) 

Instance Method

# makeFunction(descriptor:completionHandler:)

Asynchronously creates an object representing a shader function, using the specified descriptor.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
func makeFunction(
    descriptor: MTLFunctionDescriptor,
    completionHandler: @escaping ((any MTLFunction)?, (any Error)?) -> Void
)
```

``` source
func makeFunction(descriptor: MTLFunctionDescriptor) async throws -> any MTLFunction
```

**Required**

## Parameters 

`descriptor`  

The description of the function object to create.

`completionHandler`  

A Swift closure or an Objective-C block that Metal calls after it creates the function.

## See Also

### Creating Shader Function Objects

func makeFunction(name: String) -> (any MTLFunction)?

Creates an object that represents a shader function in the library.

**Required**

func makeFunction(name: String, constantValues: MTLFunctionConstantValues, completionHandler: ((any MTLFunction)?, (any Error)?) -> Void)

Asynchronously creates a specialized shader function.

**Required**

func makeFunction(name: String, constantValues: MTLFunctionConstantValues) throws -> any MTLFunction

Synchronously creates a specialized shader function.

**Required**

func makeFunction(descriptor: MTLFunctionDescriptor) throws -> any MTLFunction

Synchronously creates an object representing a shader function, using the specified descriptor.

**Required**

