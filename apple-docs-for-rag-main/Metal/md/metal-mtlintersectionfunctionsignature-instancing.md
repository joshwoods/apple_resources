

- Metal
- MTLIntersectionFunctionSignature
-  instancing 

Type Property

# instancing

A flag indicating that function signature uses instancing.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 16.0+visionOS 1.0+

``` source
static var instancing: MTLIntersectionFunctionSignature { get }
```

## Discussion

The corresponding MSL function must contain the `instancing` tag in its declaration.

## See Also

### Specifying the Intersection Function Signature

static var triangleData: MTLIntersectionFunctionSignature

A flag indicating that function signature uses triangle data.

static var worldSpaceData: MTLIntersectionFunctionSignature

A flag indicating that function signature uses world space data.

