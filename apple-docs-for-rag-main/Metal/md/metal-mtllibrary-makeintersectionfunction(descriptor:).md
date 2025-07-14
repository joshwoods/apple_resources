

- Metal
- MTLLibrary
-  makeIntersectionFunction(descriptor:) 

Instance Method

# makeIntersectionFunction(descriptor:)

Synchronously creates an object representing a ray-tracing intersection function, using the specified descriptor.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 16.0+visionOS 1.0+

``` source
func makeIntersectionFunction(descriptor: MTLIntersectionFunctionDescriptor) throws -> any MTLFunction
```

**Required**

## See Also

### Creating Intersection Function Objects

func makeIntersectionFunction(descriptor: MTLIntersectionFunctionDescriptor, completionHandler: ((any MTLFunction)?, (any Error)?) -> Void)

Asynchronously creates an object representing a ray-tracing intersection function, using the specified descriptor.

**Required**

