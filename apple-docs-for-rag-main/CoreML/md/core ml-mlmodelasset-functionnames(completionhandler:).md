

- Core ML
- MLModelAsset
-  functionNames(completionHandler:) 

Instance Method

# functionNames(completionHandler:)

The list of function names in the model asset.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
func functionNames(completionHandler handler: @escaping ([String]?, (any Error)?) -> Void)
```

``` source
var functionNames: [String] { get async throws }
```

## Discussion

Some model types (e.g. ML Program) supports multiple functions. Use this method to query the function names.

The method vends the empty array when the model doesn’t use the multi-function configuration.

```
let modelAsset = try MLModelAsset(url: modelURL)
let functionNames = try await modelAsset.functionNames
print(functionNames) // For example, ["my_function1", "my_function2"];
```

