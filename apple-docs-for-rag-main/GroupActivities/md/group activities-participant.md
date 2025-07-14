

- Group Activities
-  Participant 

Structure

# Participant

An active participant in a group session.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+

``` source
struct Participant
```

## Mentioned in 

Synchronizing data during a SharePlay activity

## Overview

Use a `Participant` object to differentiate among users in a session. A participant object doesn’t contain any sensitive data about the user, but provides a unique identifier to distinguish the user while the session is active.

You don’t create participant objects directly. The system creates a participant object for each user that joins an activity. Access the current set of participants from the activeParticipants property of the GroupSession object associated with the activity.

## Topics

### Getting the unique identifier

let id: UUID

A globally unique identifier for the session participant.

### Comparing participants

static func != (Self, Self) -> Bool

Returns a Boolean value indicating whether two values are not equal.

static func == (Participant, Participant) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Instance Properties

var hashValue: Int

The hash value.

### Instance Methods

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

### Type Aliases

typealias ID

A type representing the stable identity of the entity associated with an instance.

### Default Implementations

CustomStringConvertible Implementations

Equatable Implementations

## Relationships

### Conforms To

- Copyable
- CustomStringConvertible
- Equatable
- Hashable
- Identifiable
- Sendable

## See Also

### Session management

Joining and managing a shared activity

Configure the session when a SharePlay activity starts, and handle events that occur during the lifetime of the activity.

Drawing content in a group session

Invite your friends to draw on a shared canvas while on a FaceTime call.

class GroupSession

A session for an in-progress activity that synchronizes content among participant devices.

protocol CustomMessageIdentifiable

A type that assigns a custom ID string to messages you send to other devices.

