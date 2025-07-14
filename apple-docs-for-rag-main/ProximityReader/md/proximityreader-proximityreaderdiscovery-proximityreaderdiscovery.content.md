

- ProximityReader
- ProximityReaderDiscovery
-  ProximityReaderDiscovery.Content 

Structure

# ProximityReaderDiscovery.Content

A type that represents content you can display on the current device.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+visionOS 2.0+

``` source
struct Content
```

## Overview

This structure stores information the system needs to present the appropriate interface. Don’t create instances of this structure directly. Instead, fetch each instance using the content(for:) method.

Pass instances of this structure to presentContent(_:from:) to display the associated content.

## Topics

### Getting the content identifier

let id: String

The unique identifier of the content.

### Getting the content description

let description: String

The description of the content.

### Type Aliases

typealias ID

A type representing the stable identity of the entity associated with an instance.

## Relationships

### Conforms To

- Identifiable
- Sendable

## See Also

### Fetching the content to display

func content(for: ProximityReaderDiscovery.Topic) async throws -> ProximityReaderDiscovery.Content

Fetches the content for the specified topic.

enum Topic

The topics you can present to someone.

var contentList: [ProximityReaderDiscovery.Content]

The content you can present for the current device.

