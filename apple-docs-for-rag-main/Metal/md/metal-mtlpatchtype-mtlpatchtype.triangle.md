

- Metal
- MTLPatchType
-  MTLPatchType.triangle 

Case

# MTLPatchType.triangle

A triangle patch.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+

``` source
case triangle
```

## Discussion

Metal uses this value if the shader is a post-tessellation vertex function with the `[[patch(triangle)]]` attribute.

## See Also

### Patch types

case none

An option that indicates that this isn’t a post-tessellation vertex function.

case quad

A quad patch.

