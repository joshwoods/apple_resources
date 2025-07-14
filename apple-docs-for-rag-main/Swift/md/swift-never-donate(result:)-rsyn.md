

- Swift
- Never
-  donate(result:) 

Instance Method

# donate(result:)

Donates the intent and optional result to the transcript.

SwiftAppIntentsiOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
@discardableResult
func donate(result: some IntentResult) -> IntentDonationIdentifier
```

## Discussion

This synchronous method is available to applications that haven’t adopted Swift async concurrency. The system ignores any exceptions encountered when donating this intent.

