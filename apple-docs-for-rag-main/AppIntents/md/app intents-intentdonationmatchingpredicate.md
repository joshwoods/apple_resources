

- App Intents
-  IntentDonationMatchingPredicate 

Structure

# IntentDonationMatchingPredicate

The match conditions that identify a set of previously donated app intents.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
struct IntentDonationMatchingPredicate
```

## Topics

### Creating a predicate

static func donationIdentifier(IntentDonationIdentifier) -> IntentDonationMatchingPredicate

Delete the transcript record with the given donation identifier

static func entityIdentifier(EntityIdentifier) -> IntentDonationMatchingPredicate

Delete all transcript records referencing the given AppEntity instance

static func intentType(any AppIntent.Type, entityIdentifier: EntityIdentifier?) -> IntentDonationMatchingPredicate

Delete all transcript records for the given AppIntent type, optionally only those referencing a given AppEntity instance identifier

## See Also

### Donation management

struct IntentDonationManager

A type you use to donate intents to the system, or delete intents when they become irrelevant.

struct IntentDonationIdentifier

An opaque type that identifies a specific donation to the system.

