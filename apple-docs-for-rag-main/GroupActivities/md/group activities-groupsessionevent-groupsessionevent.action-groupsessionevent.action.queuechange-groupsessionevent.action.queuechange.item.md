

- Group Activities
- GroupSessionEvent
- GroupSessionEvent.Action
- GroupSessionEvent.Action.QueueChange
-  GroupSessionEvent.Action.QueueChange.Item 

Structure

# GroupSessionEvent.Action.QueueChange.Item

Detailed information about an item involved in a queue change.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+

``` source
struct Item
```

## Overview

Before you notify a participant about a queue-related change, create an item that contains the name of the song or container that changed. Use this item to configure a GroupSessionEvent.Action.QueueChange structure with additional details about the change.

## Topics

### Creating the item

static func song(String) -> GroupSessionEvent.Action.QueueChange.Item

Creates an item that contains the name of a song.

static func container(String) -> GroupSessionEvent.Action.QueueChange.Item

Creates an item that contains the name of a container.

