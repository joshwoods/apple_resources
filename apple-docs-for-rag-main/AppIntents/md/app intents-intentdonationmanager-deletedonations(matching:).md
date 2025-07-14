

- App Intents
- IntentDonationManager
-  deleteDonations(matching:) 

Instance Method

# deleteDonations(matching:)

Deletes all transcript records matching the given predicate and returns their identifiers.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
@discardableResult
func deleteDonations(matching predicate: IntentDonationMatchingPredicate) async throws -> [IntentDonationIdentifier]
```

