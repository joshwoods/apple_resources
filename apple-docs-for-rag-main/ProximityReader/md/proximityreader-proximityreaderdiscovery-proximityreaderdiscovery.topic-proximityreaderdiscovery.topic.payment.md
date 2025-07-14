

- ProximityReader
- ProximityReaderDiscovery
- ProximityReaderDiscovery.Topic
-  ProximityReaderDiscovery.Topic.Payment 

Enumeration

# ProximityReaderDiscovery.Topic.Payment

The subtopics that show merchants how to accept different types of payments with *Tap to Pay* on iPhone.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+visionOS 2.0+

``` source
enum Payment
```

## Overview

Each topic has a dedicated learning purpose for merchants.

## Topics

### Operators

static func == (ProximityReaderDiscovery.Topic.Payment, ProximityReaderDiscovery.Topic.Payment) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Enumeration Cases

case howToTap

A topic that shows merchants how to use Tap to Pay on iPhone to pay for goods and services.

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

- Copyable
- Equatable
- Hashable
- Sendable

## See Also

### Creating a discovery object

case payment(ProximityReaderDiscovery.Topic.Payment)

A topic related to accepting payments.

