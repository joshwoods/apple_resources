

- AVFoundation
- AVMetadataItem
-  dataType 

Instance Property

# dataType

The data type of the metadata item’s value.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 1.0+

``` source
var dataType: String? { get }
```

## See Also

### Loading Values

static var value: AVAsyncProperty&lt;Root, (any NSCopying &amp; NSObjectProtocol)?>

The value of the metadata item.

static var stringValue: AVAsyncProperty&lt;Root, String?>

The value of the metadata item as a string.

static var numberValue: AVAsyncProperty&lt;Root, NSNumber?>

The value of the metadata item as a number.

static var dateValue: AVAsyncProperty&lt;Root, Date?>

The value of the metadata item as a date.

static var dataValue: AVAsyncProperty&lt;Root, Data?>

The value of the metadata item as a data value.

static var extraAttributes: AVAsyncProperty&lt;Root, [AVMetadataExtraAttributeKey : Any]?>

A dictionary of additional attributes for the item.

