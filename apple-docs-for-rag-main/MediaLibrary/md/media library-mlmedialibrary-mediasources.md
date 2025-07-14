

- Media Library
- MLMediaLibrary
-  mediaSources 

Instance Property

# mediaSources

Returns a dictionary of media sources by identifier.

Mac Catalyst 13.0+macOS 10.9–10.15Deprecated

``` source
var mediaSources: [String : MLMediaSource]? { get }
```

## Discussion

Returns `nil` the first time, beginning an asynchronous load of the media sources. A KVO notification is sent when all media sources have been loaded. If there are no objects in a media source, the source does not appear in this dictionary.

