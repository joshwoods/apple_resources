

- Swift
- Task
-  withGroup(resultType:returning:body:) Deprecated

Type Method

# withGroup(resultType:returning:body:)

iOS 13.0+iPadOS 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+Mac Catalyst 13.0+

``` source
static func withGroup(
    resultType: TaskResult.Type,
    returning returnType: BodyResult.Type = BodyResult.self,
    body: (inout Task.Group) async throws -> BodyResult
) async rethrows -> BodyResult where TaskResult : Sendable
```

Available when `Success` is `Never` and `Failure` is `Never`.

Deprecated

\`Task.withGroup\` was replaced by \`withThrowingTaskGroup\` and \`withTaskGroup\` and will be removed shortly.

