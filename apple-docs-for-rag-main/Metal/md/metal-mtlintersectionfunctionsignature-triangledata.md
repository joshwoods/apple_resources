

- Metal
- MTLIntersectionFunctionSignature
-  triangleData 

Type Property

# triangleData

A flag indicating that function signature uses triangle data.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 16.0+visionOS 1.0+

``` source
static var triangleData: MTLIntersectionFunctionSignature { get }
```

## Discussion

The corresponding MSL function must contain the `triangle_data` tag in its declaration.

## See Also

### Specifying the Intersection Function Signature

static var instancing: MTLIntersectionFunctionSignature

A flag indicating that function signature uses instancing.

static var worldSpaceData: MTLIntersectionFunctionSignature

A flag indicating that function signature uses world space data.

