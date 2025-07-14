

- AVFoundation
-  AVPlayerItemMetadataCollector 

Class

# AVPlayerItemMetadataCollector

An object used to capture the date range metadata defined for an HTTP Live Streaming asset.

iOS 9.3+iPadOS 9.3+Mac Catalyst 13.1+macOS 10.11.3+tvOS 9.2+visionOS 1.0+watchOS 2.3+

``` source
class AVPlayerItemMetadataCollector
```

## Overview

You can use the HLS `#EXT-X-DATERANGE` tag to define date range metadata in a media playlist. This tag is useful for defining timed metadata for interstitial regions such as advertisements, but can be used to define any timed metadata needed by your stream. To access this metadata when the stream is played using an AVPlayer, you create an instance of `AVPlayerItemMetadataCollector`, configure its delegate object (see AVPlayerItemMetadataCollectorPushDelegate), and add it as a media data collector to the AVPlayerItem (see example).

- Swift
- Objective-C

```
class PlaybackController: NSObject, AVPlayerItemMetadataCollectorPushDelegate {

    let player = AVPlayer()
    var playerItem: AVPlayerItem!
    var metadataCollector: AVPlayerItemMetadataCollector!

    func prepareToPlay(url: URL) {
        metadataCollector = AVPlayerItemMetadataCollector()
        metadataCollector.setDelegate(self, queue: DispatchQueue.main)

        playerItem = AVPlayerItem(url: url)
        playerItem.add(metadataCollector)

        player.replaceCurrentItem(with: playerItem)
    }

    func metadataCollector(_ metadataCollector: AVPlayerItemMetadataCollector,
                           didCollect metadataGroups: [AVDateRangeMetadataGroup],
                           indexesOfNewGroups: IndexSet,
                           indexesOfModifiedGroups: IndexSet) {
        // Process metadata
    }
}
```

```
// Adopts AVPlayerItemMetadataCollectorPushDelegate
@implementation PlaybackController

- (void)prepareToPlay:(NSURL *)url {
    self.metadataCollector = [[AVPlayerItemMetadataCollector alloc] init];
    [self.metadataCollector setDelegate:self queue:dispatch_get_main_queue()];

    self.playerItem = [AVPlayerItem playerItemWithURL:url];
    [self.playerItem addMediaDataCollector:self.metadataCollector];

    self.player = [AVPlayer playerWithPlayerItem:self.playerItem];
}

- (void)metadataCollector:(AVPlayerItemMetadataCollector *)metadataCollector
didCollectDateRangeMetadataGroups:(NSArray *)metadataGroups
       indexesOfNewGroups:(NSIndexSet *)indexesOfNewGroups
  indexesOfModifiedGroups:(NSIndexSet *)indexesOfModifiedGroups {
    // Process metadata
}

@end
```

Creating an `AVPlayerItemMetadataCollector` as shown in the example, will capture all `#EXT-X-DATERANGE` metadata defined in your stream. If you would like to filter the output to only the metadata of interest, you can create an instance to filter by identifier and/or classifying labels using the init(identifiers:classifyingLabels:) initializer.

## Topics

### Creating a Metadata Collector

init(identifiers: [String]?, classifyingLabels: [String]?)

Creates a metadata collector to access a stream’s metadata groups matching the specified array of identifiers and classifying labels.

### Accessing the Delegate and Callback Queue

func setDelegate((any AVPlayerItemMetadataCollectorPushDelegate)?, queue: dispatch_queue_t?)

Sets the delegate and a dispatch queue on which the delegate will be called.

var delegate: (any AVPlayerItemMetadataCollectorPushDelegate)?

Accesses the metadata collector’s delegate object.

protocol AVPlayerItemMetadataCollectorPushDelegate

A protocol you implement to receive metadata callbacks from a player item metadata collector.

var delegateQueue: dispatch_queue_t?

The dispatch queue on which the delegate’s methods are called.

## Relationships

### Inherits From

- AVPlayerItemMediaDataCollector

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol
- Sendable

## See Also

### Timed metadata

Presenting Chapter Markers

Add chapter markers to enable users to quickly navigate your content.

class AVMetadataGroup

A collection of metadata items associated with a timeline segment.

class AVTimedMetadataGroup

A collection of metadata items that are valid for use during a specific time range.

class AVMutableTimedMetadataGroup

A mutable collection of metadata items that are valid for use during a specific time range.

class AVDateRangeMetadataGroup

A collection of metadata items that are valid for use within a specific date range.

class AVMutableDateRangeMetadataGroup

A mutable collection of metadata items that are valid for use within a specific range of dates.

class AVPlayerItemMediaDataCollector

The abstract base for media data collectors.

