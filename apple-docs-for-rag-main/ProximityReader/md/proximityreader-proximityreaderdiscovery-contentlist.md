

- ProximityReader
- ProximityReaderDiscovery
-  contentList 

Instance Property

# contentList

The content you can present for the current device.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+visionOS 2.0+

``` source
final var contentList: [ProximityReaderDiscovery.Content] { get async throws }
```

## Discussion

This property contains zero or more ProximityReaderDiscovery.Content structures, each of which corresponds to information on a supported topic. The content associated with each structure is specific to the country of the current device. The array can be empty if no content is available for the current country.

Use this list only when you need to display a topic that isn’t available in ProximityReaderDiscovery.Topic. In all other cases, use the content(for:) method to fetch the topic.

Accessing this property fetches the ProximityReaderDiscovery.Content structures from the system. If the system is unable to fetch the needed information, it throws an error.

## See Also

### Fetching the content to display

func content(for: ProximityReaderDiscovery.Topic) async throws -> ProximityReaderDiscovery.Content

Fetches the content for the specified topic.

enum Topic

The topics you can present to someone.

struct Content

A type that represents content you can display on the current device.

