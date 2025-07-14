

- ProximityReader
- ProximityReaderDiscovery
-  ProximityReaderDiscovery.Topic 

Enumeration

# ProximityReaderDiscovery.Topic

The topics you can present to someone.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+visionOS 2.0+

``` source
enum Topic
```

## Topics

### Creating a discovery object

case payment(ProximityReaderDiscovery.Topic.Payment)

A topic related to accepting payments.

enum Payment

The subtopics that show merchants how to accept different types of payments with *Tap to Pay* on iPhone.

## Relationships

### Conforms To

- Sendable

## See Also

### Fetching the content to display

func content(for: ProximityReaderDiscovery.Topic) async throws -> ProximityReaderDiscovery.Content

Fetches the content for the specified topic.

struct Content

A type that represents content you can display on the current device.

var contentList: [ProximityReaderDiscovery.Content]

The content you can present for the current device.

