

- Core ML
- MLModelConfiguration
-  functionName 

Instance Property

# functionName

Function name that `MLModel` will use.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
var functionName: String? { get set }
```

## Discussion

Some model types (e.g. ML Program) supports multiple functions in a model asset, where each `MLModel` instance is associated with a particular function.

Use `MLModelAsset` to get the list of available functions. Use `nil` to use a default function.

```
let configuration = MLModelConfiguration()
configuration.functionName = "my_function"
```

