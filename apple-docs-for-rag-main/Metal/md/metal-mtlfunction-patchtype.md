

- Metal
- MTLFunction
-  patchType 

Instance Property

# patchType

The tessellation patch type of a post-tessellation vertex function.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+

``` source
var patchType: MTLPatchType { get }
```

**Required**

## Discussion

This value is MTLPatchType.none if the function isn’t a post-tessellation vertex function.

## See Also

### Identifying the Tessellation Patch

var patchControlPointCount: Int

The number of patch control points in the post-tessellation vertex function.

**Required**

enum MTLPatchType

Types of tessellation patches that can be inputs of a post-tessellation vertex function.

