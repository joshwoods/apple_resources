

- Speech
- SFSpeechLanguageModel
-  prepareCustomLanguageModel(for:clientIdentifier:configuration:completion:) 

Type Method

# prepareCustomLanguageModel(for:clientIdentifier:configuration:completion:)

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+visionOS 1.0+

``` source
class func prepareCustomLanguageModel(
    for asset: URL,
    clientIdentifier: String,
    configuration: SFSpeechLanguageModel.Configuration,
    completion: @escaping ((any Error)?) -> Void
)
```

``` source
class func prepareCustomLanguageModel(
    for asset: URL,
    clientIdentifier: String,
    configuration: SFSpeechLanguageModel.Configuration
) async throws
```

## See Also

### Type Methods

class func prepareCustomLanguageModel(for: URL, clientIdentifier: String, configuration: SFSpeechLanguageModel.Configuration, ignoresCache: Bool, completion: ((any Error)?) -> Void)

