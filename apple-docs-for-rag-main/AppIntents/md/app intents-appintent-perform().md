

- App Intents
- AppIntent
-  perform() 

Instance Method

# perform()

Performs the intent after resolving the provided parameters.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
func perform() async throws -> Self.PerformResult
```

**Required** Default implementations provided.

## Mentioned in 

Responding to the Action button on Apple Watch Ultra

Creating your first app intent

Integrating custom data types into your intents

## Discussion

In the body of this function, validate your parameters and provide the system with information about needed parameter values or user clarification.

## Default Implementations

### AppIntent Implementations

func perform() async throws -> Never

func perform() async throws -> Self.NeverResult

func perform() async throws -> Never

func perform() async throws -> some IntentResult

func perform() async throws -> Never

func perform() async throws -> Self.NeverResult

A default implementation that throws an error rather than perform an intent.

## See Also

### Performing the action

var systemContext: IntentSystemContext

Context information that’s available while the system performs the app intent’s action.

associatedtype PerformResult : IntentResult

**Required**

