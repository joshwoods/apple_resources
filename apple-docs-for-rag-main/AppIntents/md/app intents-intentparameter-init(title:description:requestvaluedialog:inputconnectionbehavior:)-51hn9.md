

- App Intents
- IntentParameter
-  init(title:description:requestValueDialog:inputConnectionBehavior:) 

Initializer

# init(title:description:requestValueDialog:inputConnectionBehavior:)

iOS 17.2+iPadOS 17.2+Mac Catalyst 17.2+macOS 14.2+tvOS 17.2+visionOS 1.0+watchOS 10.2+

``` source
convenience init(
    title: LocalizedStringResource,
    description: LocalizedStringResource? = nil,
    requestValueDialog: IntentDialog? = nil,
    inputConnectionBehavior: InputConnectionBehavior = .default
)
```

Available when `Value` conforms to `_IntentValue`, `Value` conforms to `Sendable`, and `Value.ValueType` is `StringSearchCriteria`.

