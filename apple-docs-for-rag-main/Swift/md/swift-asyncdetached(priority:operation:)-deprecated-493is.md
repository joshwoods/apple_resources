

- Swift
-  asyncDetached(priority:operation:) Deprecated

Function

# asyncDetached(priority:operation:)

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
@discardableResult
func asyncDetached(
    priority: TaskPriority? = nil,
    operation: @escaping () async throws -> T
) -> Task where T : Sendable
```

Deprecated

\`asyncDetached\` was replaced by \`Task.detached\` and will be removed shortly.

## See Also

### Deprecated Functions

func async&lt;T>(priority: TaskPriority?, operation: () async -> T) -> Task&lt;T, Never>Deprecated

func async&lt;T>(priority: TaskPriority?, operation: () async throws -> T) -> Task&lt;T, any Error>Deprecated

func asyncDetached&lt;T>(priority: TaskPriority?, operation: () async -> T) -> Task&lt;T, Never>Deprecated

func detach&lt;T>(priority: TaskPriority?, operation: () async -> T) -> Task&lt;T, Never>Deprecated

func detach&lt;T>(priority: TaskPriority?, operation: () async -> T) -> Task&lt;T, Never>Deprecated

func detach&lt;T>(priority: TaskPriority?, operation: () async throws -> T) -> Task&lt;T, any Error>Deprecated

func detach&lt;T>(priority: TaskPriority?, operation: () async throws -> T) -> Task&lt;T, any Error>Deprecated

