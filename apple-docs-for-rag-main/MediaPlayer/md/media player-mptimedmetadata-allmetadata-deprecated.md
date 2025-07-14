

- Media Player
- MPTimedMetadata
-  allMetadata Deprecated

Instance Property

# allMetadata

A dictionary containing all the metadata in the object.

iOS 3.2–9.0DeprecatediPadOS 3.2–9.0DeprecatedMac Catalyst 13.1–13.1Deprecated

``` source
var allMetadata: [AnyHashable : Any]! { get }
```

Deprecated

Use AVPlayerViewController in AVKit

## Discussion

To retrieve metadata from the dictionary, use the keys described in Timed metadata dictionary keys.

## See Also

### Extracting timed metadata from a stream

var key: String!

A key that identifies a piece of timed metadata.

Deprecated

var keyspace: String!

The namespace of the identifying key.

Deprecated

var timestamp: TimeInterval

The timestamp of the metadata, in the timebase of the media stream.

Deprecated

var value: Any!

The timed metadata.

Deprecated

