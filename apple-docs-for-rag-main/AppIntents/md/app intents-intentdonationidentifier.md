

- App Intents
-  IntentDonationIdentifier 

Structure

# IntentDonationIdentifier

An opaque type that identifies a specific donation to the system.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
struct IntentDonationIdentifier
```

## Topics

### Creating an identifier

init(from: any Decoder) throws

Creates a new instance by decoding from the given decoder.

### Encoding the type

func encode(to: any Encoder) throws

Encodes this value into the given encoder.

### Comparing identifiers

static func == (IntentDonationIdentifier, IntentDonationIdentifier) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Instance Properties

var hashValue: Int

The hash value.

### Instance Methods

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

### Default Implementations

Equatable Implementations

## Relationships

### Conforms To

- Decodable
- Encodable
- Equatable
- Hashable
- Sendable

## See Also

### Donation management

struct IntentDonationManager

A type you use to donate intents to the system, or delete intents when they become irrelevant.

struct IntentDonationMatchingPredicate

The match conditions that identify a set of previously donated app intents.

