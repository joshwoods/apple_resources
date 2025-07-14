

- Metal
- MTLStitchedLibraryDescriptor
-  functions 

Instance Property

# functions

The list of functions for creating the stitched library.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+

``` source
var functions: [any MTLFunction] { get set }
```

## Discussion

The function objects must all be created by the same Metal device object that you’ll use to create the library. The MSL functions referenced by these function objects must be declared with the `stitchable` attribute, as in the example below:

```
[[stitchable]]
 float add(float a, float b)
{
    return a + b;
}
```

## See Also

### Configuring a Stitched Library

var functionGraphs: [MTLFunctionStitchingGraph]

The function graphs that define the new stitched library’s functions.

