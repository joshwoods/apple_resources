

- App Intents
- AppIntent
-  PerformResult 

Associated Type

# PerformResult

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
associatedtype PerformResult : IntentResult
```

**Required**

## See Also

### Performing the action

func perform() async throws -> Self.PerformResult

Performs the intent after resolving the provided parameters.

**Required** Default implementations provided.

var systemContext: IntentSystemContext

Context information that’s available while the system performs the app intent’s action.

