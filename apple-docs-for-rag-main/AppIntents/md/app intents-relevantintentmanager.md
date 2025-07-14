

- App Intents
-  RelevantIntentManager 

Class

# RelevantIntentManager

A type that saves relevant intents.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
final class RelevantIntentManager
```

## Topics

### Instance Methods

func updateRelevantIntents([RelevantIntent]) async throws

Give the system the list of relevant intents for your app. To replace the list, call this method again, passing in a new list of relevant intents. To remove all relevant intents associated with your app, call this method with an empty array.

### Type Properties

static let shared: RelevantIntentManager

Get the singleton shared instance of this class.

## See Also

### Intent relevancy

struct RelevantIntent

A type that specifies an intent and its relevance to the user.

struct RelevantContext

A type that specifies conditions for relevance.

