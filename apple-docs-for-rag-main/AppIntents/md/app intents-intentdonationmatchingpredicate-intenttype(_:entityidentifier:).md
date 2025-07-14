

- App Intents
- IntentDonationMatchingPredicate
-  intentType(\_:entityIdentifier:) 

Type Method

# intentType(\_:entityIdentifier:)

Delete all transcript records for the given AppIntent type, optionally only those referencing a given AppEntity instance identifier

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
static func intentType(
    _ intentType: any AppIntent.Type,
    entityIdentifier: EntityIdentifier? = nil
) -> IntentDonationMatchingPredicate
```

## See Also

### Creating a predicate

static func donationIdentifier(IntentDonationIdentifier) -> IntentDonationMatchingPredicate

Delete the transcript record with the given donation identifier

static func entityIdentifier(EntityIdentifier) -> IntentDonationMatchingPredicate

Delete all transcript records referencing the given AppEntity instance

