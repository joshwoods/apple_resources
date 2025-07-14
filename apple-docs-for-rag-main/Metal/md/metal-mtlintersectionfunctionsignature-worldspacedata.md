

- Metal
- MTLIntersectionFunctionSignature
-  worldSpaceData 

Type Property

# worldSpaceData

A flag indicating that function signature uses world space data.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 16.0+visionOS 1.0+

``` source
static var worldSpaceData: MTLIntersectionFunctionSignature { get }
```

## Discussion

The corresponding MSL function must contain the `world_space_data` tag in its declaration.

## See Also

### Specifying the Intersection Function Signature

static var instancing: MTLIntersectionFunctionSignature

A flag indicating that function signature uses instancing.

static var triangleData: MTLIntersectionFunctionSignature

A flag indicating that function signature uses triangle data.

