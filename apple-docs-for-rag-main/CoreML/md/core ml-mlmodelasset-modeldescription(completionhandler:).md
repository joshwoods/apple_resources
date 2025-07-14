

- Core ML
- MLModelAsset
-  modelDescription(completionHandler:) 

Instance Method

# modelDescription(completionHandler:)

The default model descripton.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
func modelDescription(completionHandler handler: @escaping (MLModelDescription?, (any Error)?) -> Void)
```

``` source
var modelDescription: MLModelDescription { get async throws }
```

## Discussion

Use this method to get the description of the model such as the feature descriptions, the model author, and other metadata.

For the multi-function model asset, this method vends the description for the default function. Use `modelDescription(for:)` to get the model description of other functions.

```
let modelAsset = try MLModelAsset(url: modelURL)
let modelDescription = try await modelAsset.modelDescription()
print(modelDescription)
```

