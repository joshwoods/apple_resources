

- App Intents
- IntentDonationManager
-  donate(intent:result:) 

Instance Method

# donate(intent:result:)

Donates an AppIntent and IntentResult to the transcript.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
@discardableResult
func donate(
    intent: some AppIntent,
    result: some IntentResult
) async throws -> IntentDonationIdentifier
```

