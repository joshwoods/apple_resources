

- ProximityReader
-  StoreAndForwardStatus 

Structure

# StoreAndForwardStatus

A structure that describes the Store and Forward session status.

iOS 18.4+iPadOS 18.4+Mac Catalyst 18.4+visionOS 2.4+

``` source
struct StoreAndForwardStatus
```

## Overview

A session’s `StoreAndForwardStatus` tells you when the Store and Forward session expires and how many successful reads the framework performed using a Store and Forward session.

Call status() to get the current Store and Forward status for your device.

## Topics

### Operators

static func == (StoreAndForwardStatus, StoreAndForwardStatus) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Instance Properties

let expiration: Date

The date when the Store and Forward session expires.

var hashValue: Int

The hash value.

let readCount: Int

The number of successful reads the framework performed using a Store and Forward session.

### Instance Methods

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

### Default Implementations

Equatable Implementations

## Relationships

### Conforms To

- Equatable
- Hashable
- Sendable

