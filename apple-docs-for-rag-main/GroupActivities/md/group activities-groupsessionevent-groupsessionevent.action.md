

- Group Activities
- GroupSessionEvent
-  GroupSessionEvent.Action 

Structure

# GroupSessionEvent.Action

A playback-related change that occurs during the session.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+

``` source
struct Action
```

## Overview

Use this structure to communicate playback-related changes to participants using the system UI. You can use this structure to communicate the following types of events:

- Transport-related events for a custom player.

- Changes to a playback queue your app manages.

When a change occurs in your custom player or playback queue, create an instance of this structure to describe the change and wrap it in a GroupSessionEvent structure. To display the event to the participant call the showNotice(_:) method of the session. The system formats and displays the information you provide.

Note

If your app uses AV Foundation to play content, you don’t need to communicate transport-related events yourself. AV Foundation generates appropriate events when the user plays, pauses, seeks, or skips tracks.

## Topics

### Getting playback-related actions

static let play: GroupSessionEvent.Action

An action that indicates the start of playback.

static let pause: GroupSessionEvent.Action

An action that indicates an end to playback.

static let seek: GroupSessionEvent.Action

An event that indicates a change to the current playback location.

static func skip(item: String) -> GroupSessionEvent.Action

Returns an event that indicates a skipped track or playback item.

### Getting change-related actions

static func updatedQueue(GroupSessionEvent.Action.QueueChange) -> GroupSessionEvent.Action

Returns an action that represents a change to the playback queue.

static let updatedQueue: GroupSessionEvent.Action

An action that represents a nonspecific change to the queue.

struct QueueChange

A type that describes a modification to the playback queue.

## See Also

### Getting the event details

let originator: Participant

The participant that initiated the event.

let url: URL?

The URL to open when the participant taps the event link in the system UI.

let action: GroupSessionEvent.Action

The reason for the event.

