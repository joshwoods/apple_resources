

- ClassKit
- CLSContext
-  topic 

Instance Property

# topic

The area of study to which a context relates.

iOS 11.3+iPadOS 11.3+Mac Catalyst 11.3+macOS 11.0+visionOS 1.0+

``` source
var topic: CLSContextTopic? { get set }
```

## Discussion

Set the topic to tell teachers what kind of content a given context covers using one of the values from CLSContextTopic. The topic set on a context applies to that context and any of its descendants for which you haven’t explicitly set a topic. So if your entire app covers only a single topic, you only need to set the topic for the mainAppContext.

## See Also

### Managing context presentation

var displayOrder: Int

The position of a context relative to its siblings.

struct CLSContextTopic

The areas of study to which contexts may relate.

