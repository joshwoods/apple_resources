

- App Intents
- AppIntent
-  callAsFunction(donate:) 

Instance Method

# callAsFunction(donate:)

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
func callAsFunction(donate donateOnCompletion: Bool = true) async throws where Self.PerformResult.Value == Never
```

## See Also

### Donating the intent to the system

func donate() async throws -> IntentDonationIdentifier

Donates the intent to the transcript.

func donate() -> IntentDonationIdentifier

Donates the intent to the transcript.

func donate(result: some IntentResult) async throws -> IntentDonationIdentifier

Donates the intent and optional result to the transcript.

func donate(result: some IntentResult) -> IntentDonationIdentifier

Donates the intent and optional result to the transcript.

func callAsFunction(donate: Bool) async throws -> Self.PerformResult.Value

