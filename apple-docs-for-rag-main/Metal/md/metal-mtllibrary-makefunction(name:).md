

- Metal
- MTLLibrary
-  makeFunction(name:) 

Instance Method

# makeFunction(name:)

Creates an object that represents a shader function in the library.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.11+tvOSvisionOS 1.0+

``` source
func makeFunction(name functionName: String) -> (any MTLFunction)?
```

**Required**

## Parameters 

`functionName`  

The name of the function.

## Return Value

A MTLFunction, or `nil` if the named function isn’t found in the library.

## Discussion

If you call this method to retrieve a function that doesn’t use function constants, it returns a MTLFunction object that you can use to build a render or compute pipeline.

If you call this method to retrieve a function that uses function constants to specialize its behavior, you can only use the returned object to query the `functionConstants` property for the list of function constants. You can’t use to create a render or compute pipeline. To get a specialized object that you can use to create a pipeline object, call the makeFunction(name:constantValues:completionHandler:) method or makeFunction(name:constantValues:) to generate a specialized function.

## See Also

### Related Documentation

Metal Shading Language Guide

Metal Programming Guide

### Creating Shader Function Objects

func makeFunction(name: String, constantValues: MTLFunctionConstantValues, completionHandler: ((any MTLFunction)?, (any Error)?) -> Void)

Asynchronously creates a specialized shader function.

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

