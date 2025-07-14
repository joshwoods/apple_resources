

- Metal
- MTLLinkedFunctions
-  privateFunctions 

Instance Property

# privateFunctions

An array of function objects to link to the new function, without exporting the functions publicly.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+

``` source
var privateFunctions: [any MTLFunction]? { get set }
```

## Discussion

These functions are not exported by the pipeline state as MTLFunctionHandle objects. The Metal device object doesn’t need to support function pointers to link private functions.

## See Also

### Specifying Related Functions

var functions: [any MTLFunction]?

An array of function objects to link to the new function.

var binaryFunctions: [any MTLFunction]?

An array of function objects already compiled to a binary representation to link.

var groups: [String : [any MTLFunction]]?

An optional list of groups specifying which functions your shader can call at each call site.

