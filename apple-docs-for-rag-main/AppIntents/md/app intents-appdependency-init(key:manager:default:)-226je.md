

- App Intents
- AppDependency
-  init(key:manager:default:) 

Initializer

# init(key:manager:default:)

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
convenience init(
    key: AnyHashable? = nil,
    manager: AppDependencyManager = .shared,
    default defaultValueProvider: @escaping () async throws -> Value
)
```

