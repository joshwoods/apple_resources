

- AVFoundation
- AVPartialAsyncProperty
-  dataValue 

Type Property

# dataValue

The value of the metadata item as a data value.

iOS 15.0+iPadOS 15.0+Mac CatalystmacOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
static var dataValue: AVAsyncProperty { get }
```

Available when `Root` inherits `AVMetadataItem`.

## Mentioned in 

Retrieving media metadata

## Discussion

Use the load(_:) method to retrieve the property value.

## See Also

### Loading Values

var dataType: String?

The data type of the metadata item’s value.

static var value: AVAsyncProperty&lt;Root, (any NSCopying &amp; NSObjectProtocol)?>

The value of the metadata item.

static var stringValue: AVAsyncProperty&lt;Root, String?>

The value of the metadata item as a string.

static var numberValue: AVAsyncProperty&lt;Root, NSNumber?>

The value of the metadata item as a number.

static var dateValue: AVAsyncProperty&lt;Root, Date?>

The value of the metadata item as a date.

static var extraAttributes: AVAsyncProperty&lt;Root, [AVMetadataExtraAttributeKey : Any]?>

A dictionary of additional attributes for the item.

