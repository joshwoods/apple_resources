

- Group Activities
- GroupSession
-  GroupSession.Event 

Structure

# GroupSession.Event

A session-related event to display in the system UI.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+

``` source
struct Event
```

Available when `ActivityType` conforms to `GroupActivity`.

## Overview

Use this structure to specify the contents of custom activity-related events. The AV Foundation framework posts media-related events to the system on your app’s behalf; create an instance of this structure if your app posts additional events that don’t route through AV Foundation.

After creating an instance of this structure, post it to the system using the showNotice(_:) method of GroupSession.

## Topics

### Getting the event details

let originator: Participant

The participant that initiated the event.

Deprecated

### Initializers

init(originator: Participant, localizedDescription: String)Deprecated

### Instance Properties

var localizedDescription: String

A localized description of the event

Deprecated

