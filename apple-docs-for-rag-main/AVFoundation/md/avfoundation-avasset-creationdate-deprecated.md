

- AVFoundation
- AVAsset
-  creationDate Deprecated

Instance Property

# creationDate

A metadata item that indicates the asset’s creation date.

iOS 5.0–16.0DeprecatediPadOS 5.0–16.0DeprecatedMac Catalyst 13.1–16.0DeprecatedmacOS 10.8–13.0DeprecatedtvOS 9.0–16.0DeprecatedwatchOS 1.0–9.0Deprecated

``` source
var creationDate: AVMetadataItem? { get }
```

Deprecated

Load the value of creationDate asynchronously instead.

## Discussion

If the asset contains metadata that the framework can convert to an NSDate, you can retrieve it from the metadata item using its dateValue property. Otherwise, you retrieve it as a string by using the metadata item’s stringValue property.

This property value is `nil` if no creation date metadata exists.

