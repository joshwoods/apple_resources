

- App Intents
-  IntentDonationManager 

Structure

# IntentDonationManager

A type you use to donate intents to the system, or delete intents when they become irrelevant.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
struct IntentDonationManager
```

## Topics

### Getting the donation manager

static var shared: IntentDonationManager

### Deleting previous donations

func deleteDonations(matching: IntentDonationMatchingPredicate) async throws -> [IntentDonationIdentifier]

Deletes all transcript records matching the given predicate and returns their identifiers.

### Instance Methods

func donate(intent: some AppIntent) -> IntentDonationIdentifier

Donates an AppIntent to the transcript.

func donate(intent: some AppIntent) async throws -> IntentDonationIdentifier

Donates an AppIntent to the transcript.

func donate(intent: some AppIntent, result: some IntentResult) async throws -> IntentDonationIdentifier

Donates an AppIntent and IntentResult to the transcript.

func donate(intent: some AppIntent, result: some IntentResult) -> IntentDonationIdentifier

Donates an AppIntent and IntentResult to the transcript.

## See Also

### Donation management

struct IntentDonationIdentifier

An opaque type that identifies a specific donation to the system.

struct IntentDonationMatchingPredicate

The match conditions that identify a set of previously donated app intents.

