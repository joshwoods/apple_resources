

- Metal
- MTLIntersectionFunctionTable
-  setOpaqueTriangleIntersectionFunction(signature:index:) 

Instance Method

# setOpaqueTriangleIntersectionFunction(signature:index:)

Sets an entry in the intersection table to point to a system-defined opaque triangle intersection function.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 16.0+visionOS 1.0+

``` source
func setOpaqueTriangleIntersectionFunction(
    signature: MTLIntersectionFunctionSignature,
    index: Int
)
```

**Required**

## Parameters 

`signature`  

The signature of the function.

`index`  

The index in the table to change.

## See Also

### Specifying Opaque Triangle Intersection Testing

func setOpaqueTriangleIntersectionFunction(signature: MTLIntersectionFunctionSignature, range: NSRange)

Sets a range of entries in the intersection table to point to a system-defined opaque triangle intersection function.

**Required**

