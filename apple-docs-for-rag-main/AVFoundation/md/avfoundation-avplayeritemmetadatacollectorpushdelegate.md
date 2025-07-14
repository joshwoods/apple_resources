

- AVFoundation
-  AVPlayerItemMetadataCollectorPushDelegate 

Protocol

# AVPlayerItemMetadataCollectorPushDelegate

A protocol you implement to receive metadata callbacks from a player item metadata collector.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
protocol AVPlayerItemMetadataCollectorPushDelegate : NSObjectProtocol, Sendable
```

## Topics

### Accessing HLS Date Range Metadata

func metadataCollector(AVPlayerItemMetadataCollector, didCollect: [AVDateRangeMetadataGroup], indexesOfNewGroups: IndexSet, indexesOfModifiedGroups: IndexSet)

Tells the delegate the collected metadata group information has changed and needs to be updated.

**Required**

## Relationships

### Inherits From

- NSObjectProtocol
- Sendable

## See Also

### Accessing the Delegate and Callback Queue

func setDelegate((any AVPlayerItemMetadataCollectorPushDelegate)?, queue: dispatch_queue_t?)

Sets the delegate and a dispatch queue on which the delegate will be called.

var delegate: (any AVPlayerItemMetadataCollectorPushDelegate)?

Accesses the metadata collector’s delegate object.

var delegateQueue: dispatch_queue_t?

The dispatch queue on which the delegate’s methods are called.

