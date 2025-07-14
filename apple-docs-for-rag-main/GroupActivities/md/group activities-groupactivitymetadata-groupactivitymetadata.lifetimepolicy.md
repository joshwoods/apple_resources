

- Group Activities
- GroupActivityMetadata
-  GroupActivityMetadata.LifetimePolicy 

Structure

# GroupActivityMetadata.LifetimePolicy

An activity lifetime policy used by a Group Activity.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+

``` source
struct LifetimePolicy
```

## Overview

Activities that share content owned by the initiator may wish to customize their lifetime policy so that the activity ends when the initiator leaves.

## Topics

### Operators

static func == (GroupActivityMetadata.LifetimePolicy, GroupActivityMetadata.LifetimePolicy) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Instance Properties

var hashValue: Int

The hash value.

### Instance Methods

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

### Type Properties

static let automatic: GroupActivityMetadata.LifetimePolicy

The default lifetime policy for a group activity.

static let endsWhenInitiatorLeaves: GroupActivityMetadata.LifetimePolicy

The activity should end when the initiator of the activity leaves.

### Default Implementations

Equatable Implementations

## Relationships

### Conforms To

- Equatable
- Hashable
- Sendable

