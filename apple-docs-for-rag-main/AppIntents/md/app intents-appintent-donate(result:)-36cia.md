

- App Intents
- AppIntent
-  donate(result:) 

Instance Method

# donate(result:)

Donates the intent and optional result to the transcript.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
@discardableResult
func donate(result: some IntentResult) async throws -> IntentDonationIdentifier
```

## See Also

### Donating the intent to the system

func donate() async throws -> IntentDonationIdentifier

Donates the intent to the transcript.

func donate() -> IntentDonationIdentifier

Donates the intent to the transcript.

func donate(result: some IntentResult) -> IntentDonationIdentifier

Donates the intent and optional result to the transcript.

func callAsFunction(donate: Bool) async throws -> Self.PerformResult.Value

func callAsFunction(donate: Bool) async throws

