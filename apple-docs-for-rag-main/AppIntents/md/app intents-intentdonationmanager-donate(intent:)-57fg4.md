

- App Intents
- IntentDonationManager
-  donate(intent:) 

Instance Method

# donate(intent:)

Donates an AppIntent to the transcript.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
@discardableResult
func donate(intent: some AppIntent) -> IntentDonationIdentifier
```

## Discussion

This synchronous interface is available for adopting application that haven’t adopted Swift async concurrency. Any exceptions encountered in donating this intent are ignored.

