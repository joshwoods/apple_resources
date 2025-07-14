

- Metal
- MTLRenderPipelineReflection
-  vertexArguments Deprecated

Instance Property

# vertexArguments

An array of argument instances, each of which represent a parameter of the pipeline state’s vertex shader.

iOS 8.0–16.0DeprecatediPadOS 8.0–16.0DeprecatedMac Catalyst 13.1–16.0DeprecatedmacOS 10.11–13.0DeprecatedtvOSDeprecatedvisionOS 1.0–1.0Deprecated

``` source
var vertexArguments: [MTLArgument]? { get }
```

Deprecated

Use vertexBindings instead.

## Discussion

The MTLArgument elements in the array are in the same order as the vertex shader’s declaration signature.

## See Also

### Deprecated

var fragmentArguments: [MTLArgument]?

An array of argument instances, each of which represent a parameter of the pipeline state’s fragment shader.

Deprecated

var tileArguments: [MTLArgument]?

An array of argument instances, each of which represent a parameter of the pipeline state’s tile shader.

Deprecated

