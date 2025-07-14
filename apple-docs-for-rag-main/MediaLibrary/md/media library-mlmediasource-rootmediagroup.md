

- Media Library
- MLMediaSource
-  rootMediaGroup 

Instance Property

# rootMediaGroup

The base media group in the media source that contains all other groups within the source as descendant elements.

Mac Catalyst 13.0+macOS 10.9–10.15Deprecated

``` source
var rootMediaGroup: MLMediaGroup? { get }
```

## Discussion

This accessor property is nonblocking. If there is no data yet, it returns `nil` and automatically triggers an internal asynchronous request. When data arrives, a KVO notification is sent via the main thread.

