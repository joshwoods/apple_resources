

- Metal
- MTLLinkedFunctions
-  functions 

Instance Property

# functions

An array of function objects to link to the new function.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
var functions: [any MTLFunction]? { get set }
```

## See Also

### Specifying Related Functions

var binaryFunctions: [any MTLFunction]?

An array of function objects already compiled to a binary representation to link.

var groups: [String : [any MTLFunction]]?

An optional list of groups specifying which functions your shader can call at each call site.

var privateFunctions: [any MTLFunction]?

An array of function objects to link to the new function, without exporting the functions publicly.

