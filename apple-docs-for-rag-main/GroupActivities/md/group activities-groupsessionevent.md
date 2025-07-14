

- Group Activities
-  GroupSessionEvent 

Structure

# GroupSessionEvent

A session-related event that appears in the system UI.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+

``` source
struct GroupSessionEvent
```

## Overview

Use this structure to specify the contents of custom activity-related events. The AV Foundation framework posts media-related events to the system on your app’s behalf; create an instance of this structure if your app posts additional events that don’t route through AV Foundation.

After creating an instance of this structure, post it to the system using the showNotice(_:) method of GroupSession.

## Topics

### Creating a group session event

init(originator: Participant, action: GroupSessionEvent.Action, url: URL?)

Creates a new event with the specified participant and action details.

### Getting the event details

let originator: Participant

The participant that initiated the event.

let url: URL?

The URL to open when the participant taps the event link in the system UI.

let action: GroupSessionEvent.Action

The reason for the event.

struct Action

A playback-related change that occurs during the session.

## See Also

### Notifying participants of playback changes

func showNotice(GroupSessionEvent)

Posts an event to the system, which displays the information in the system UI.

