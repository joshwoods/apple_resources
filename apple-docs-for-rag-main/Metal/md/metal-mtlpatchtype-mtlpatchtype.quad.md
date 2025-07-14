

- Metal
- MTLPatchType
-  MTLPatchType.quad 

Case

# MTLPatchType.quad

A quad patch.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+

``` source
case quad
```

## Discussion

Metal uses this value if the shader is a post-tessellation vertex function with the `[[patch(quad)]]` attribute.

## See Also

### Patch types

case none

An option that indicates that this isn’t a post-tessellation vertex function.

case triangle

A triangle patch.

