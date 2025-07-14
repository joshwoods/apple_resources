

- AVFoundation
- Media assets
- AVPartialAsyncProperty
-  AVMetadataItem 

API Collection

# AVMetadataItem

Asynchronous properties for metadata items.

## Topics

### Loading Values

static var value: AVAsyncProperty&lt;Root, (any NSCopying &amp; NSObjectProtocol)?>

The value of the metadata item.

static var extraAttributes: AVAsyncProperty&lt;Root, [AVMetadataExtraAttributeKey : Any]?>

A dictionary of additional attributes for the item.

static var stringValue: AVAsyncProperty&lt;Root, String?>

The value of the metadata item as a string.

static var numberValue: AVAsyncProperty&lt;Root, NSNumber?>

The value of the metadata item as a number.

static var dateValue: AVAsyncProperty&lt;Root, Date?>

The value of the metadata item as a date.

static var dataValue: AVAsyncProperty&lt;Root, Data?>

The value of the metadata item as a data value.

## See Also

### Loading Properties

AVAsset

Asynchronous properties for assets.

AVAssetTrack

Asynchronous properties for asset tracks.

AVURLAsset

Asynchronous properties for URL assets.

AVFragmentedAsset

Asynchronous properties for fragmented assets.

AVComposition

Asynchronous properties for compositions.

AVMutableComposition

Asynchronous properties for mutable compositions.

AVMovie

Asynchronous properties for movies.

AVMutableMovie

Asynchronous properties for mutable movies.

AVFragmentedMovie

Asynchronous properties for fragmented movies.

