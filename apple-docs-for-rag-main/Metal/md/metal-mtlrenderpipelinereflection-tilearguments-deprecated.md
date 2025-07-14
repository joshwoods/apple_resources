

- Metal
- MTLRenderPipelineReflection
-  tileArguments Deprecated

Instance Property

# tileArguments

An array of argument instances, each of which represent a parameter of the pipeline state’s tile shader.

iOS 11.0–16.0DeprecatediPadOS 11.0–16.0DeprecatedMac Catalyst 14.0–16.0DeprecatedmacOS 11.0–13.0DeprecatedtvOS 14.5–16.0DeprecatedvisionOS 1.0–1.0Deprecated

``` source
var tileArguments: [MTLArgument]? { get }
```

Deprecated

Use tileBindings instead.

## Discussion

The MTLArgument elements in the array are in the same order as the tile shader’s declaration signature.

## See Also

### Deprecated

var vertexArguments: [MTLArgument]?

An array of argument instances, each of which represent a parameter of the pipeline state’s vertex shader.

Deprecated

var fragmentArguments: [MTLArgument]?

An array of argument instances, each of which represent a parameter of the pipeline state’s fragment shader.

Deprecated

