

- ProximityReader
- ProximityReaderDiscovery
-  content(for:) 

Instance Method

# content(for:)

Fetches the content for the specified topic.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+visionOS 2.0+

``` source
final func content(for topic: ProximityReaderDiscovery.Topic) async throws -> ProximityReaderDiscovery.Content
```

## Parameters 

`topic`  

The topic you want to display.

## Return Value

The requested content, when successful.

## Discussion

Throws

The method throws a ProximityReaderDiscovery.ContentError if it fails to get the content.

Call this method to get the content definition for the specified topic. The discovery interface uses the specified identifier to determine what to display.

## See Also

### Fetching the content to display

enum Topic

The topics you can present to someone.

struct Content

A type that represents content you can display on the current device.

var contentList: [ProximityReaderDiscovery.Content]

The content you can present for the current device.

