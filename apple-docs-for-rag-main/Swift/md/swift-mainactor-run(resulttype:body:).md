

- Swift
- MainActor
-  run(resultType:body:) 

Type Method

# run(resultType:body:)

Execute the given body closure on the main actor.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
static func run(
    resultType: T.Type = T.self,
    body: @MainActor () throws -> T
) async rethrows -> T where T : Sendable
```

