

- Metal
- MTLComputePipelineReflection
-  arguments Deprecated

Instance Property

# arguments

An array of objects that describe the arguments of a compute function.

iOS 8.0–16.0DeprecatediPadOS 8.0–16.0DeprecatedMac Catalyst 13.1–16.0DeprecatedmacOS 10.11–13.0DeprecatedtvOSDeprecatedvisionOS 1.0–1.0Deprecated

``` source
var arguments: [MTLArgument] { get }
```

## Discussion

Each element in the array is a MTLArgument object that describes one of the function’s arguments. The elements in the array are in the same order that the arguments appear in the function declaration.

## See Also

### Related Documentation

Metal Shading Language Guide

Metal Programming Guide

