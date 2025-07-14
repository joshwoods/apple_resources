

- Media Library
- MLMediaGroup
-  mediaObjects 

Instance Property

# mediaObjects

A list of media objects in the media group.

Mac Catalyst 13.0+macOS 10.9–10.15Deprecated

``` source
var mediaObjects: [MLMediaObject]? { get }
```

## Discussion

This accessor property is nonblocking. If there is no data yet, it returns `nil` and automatically triggers an internal asynchronous request. A KVO notification will be sent via the main thread when data arrives.

## See Also

### Accessing the Group Hierarchy

var parent: MLMediaGroup?

The media group’s parent group.

var childGroups: [MLMediaGroup]?

A list of child groups contained in the media group.

