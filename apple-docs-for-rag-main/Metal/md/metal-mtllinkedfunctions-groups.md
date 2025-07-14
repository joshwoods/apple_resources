

- Metal
- MTLLinkedFunctions
-  groups 

Instance Property

# groups

An optional list of groups specifying which functions your shader can call at each call site.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
var groups: [String : [any MTLFunction]]? { get set }
```

## Discussion

The default value is `nil`.

Metal’s default behavior is conservative, it assumes that your shader can call any linked function from every call site. If you know that the shader can only call a limited subset of functions at a call site, you can annotate those sites in the shader with a name of a group and then specify the list of functions for that call site using this property. Specifying call sites and callable functions more precisely can improve performance.

For more information on how to specify call site groups, see Metal Shading Language Specification.

The value of this property is a dictionary whose keys are call site names and values are arrays specifying the list of functions that the shader can call from each site.

## See Also

### Specifying Related Functions

var functions: [any MTLFunction]?

An array of function objects to link to the new function.

var binaryFunctions: [any MTLFunction]?

An array of function objects already compiled to a binary representation to link.

var privateFunctions: [any MTLFunction]?

An array of function objects to link to the new function, without exporting the functions publicly.

