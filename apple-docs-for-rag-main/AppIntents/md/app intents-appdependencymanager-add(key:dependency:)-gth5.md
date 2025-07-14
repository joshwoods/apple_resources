

- App Intents
- AppDependencyManager
-  add(key:dependency:) 

Instance Method

# add(key:dependency:)

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
final func add(
    key: AnyHashable? = nil,
    dependency dependencyProvider: @escaping () async throws -> Dependency
) where Dependency : Sendable
```

