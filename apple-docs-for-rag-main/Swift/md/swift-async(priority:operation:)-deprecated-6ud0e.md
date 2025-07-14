

- Swift
-  async(priority:operation:) Deprecated

Function

# async(priority:operation:)

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+watchOS 6.0+visionOS 1.0+

``` source
@discardableResult
func async(
    priority: TaskPriority? = nil,
    operation: @escaping () async throws -> T
) -> Task where T : Sendable
```

Deprecated

\`async\` was replaced by \`Task.init\` and will be removed shortly.

## See Also

### Deprecated Functions

func async&lt;T>(priority: TaskPriority?, operation: () async -> T) -> Task&lt;T, Never>Deprecated

func asyncDetached&lt;T>(priority: TaskPriority?, operation: () async -> T) -> Task&lt;T, Never>Deprecated

func asyncDetached&lt;T>(priority: TaskPriority?, operation: () async throws -> T) -> Task&lt;T, any Error>Deprecated

func detach&lt;T>(priority: TaskPriority?, operation: () async -> T) -> Task&lt;T, Never>Deprecated

func detach&lt;T>(priority: TaskPriority?, operation: () async -> T) -> Task&lt;T, Never>Deprecated

func detach&lt;T>(priority: TaskPriority?, operation: () async throws -> T) -> Task&lt;T, any Error>Deprecated

func detach&lt;T>(priority: TaskPriority?, operation: () async throws -> T) -> Task&lt;T, any Error>Deprecated

