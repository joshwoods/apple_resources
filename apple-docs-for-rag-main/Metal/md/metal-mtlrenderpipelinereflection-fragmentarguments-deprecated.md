

- Metal
- MTLRenderPipelineReflection
-  fragmentArguments Deprecated

Instance Property

# fragmentArguments

An array of argument instances, each of which represent a parameter of the pipeline state’s fragment shader.

iOS 8.0–16.0DeprecatediPadOS 8.0–16.0DeprecatedMac Catalyst 13.1–16.0DeprecatedmacOS 10.11–13.0DeprecatedtvOSDeprecatedvisionOS 1.0–1.0Deprecated

``` source
var fragmentArguments: [MTLArgument]? { get }
```

Deprecated

Use fragmentBindings instead.

## Discussion

The MTLArgument elements in the array are in the same order as the fragment shader’s declaration signature.

## See Also

### Deprecated

var vertexArguments: [MTLArgument]?

An array of argument instances, each of which represent a parameter of the pipeline state’s vertex shader.

Deprecated

var tileArguments: [MTLArgument]?

An array of argument instances, each of which represent a parameter of the pipeline state’s tile shader.

Deprecated

