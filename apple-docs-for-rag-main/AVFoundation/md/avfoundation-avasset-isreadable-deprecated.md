

- AVFoundation
- AVAsset
-  isReadable Deprecated

Instance Property

# isReadable

A Boolean value that indicates whether you can extract the asset’s media data using an asset reader.

iOS 4.3–16.0DeprecatediPadOS 4.3–16.0DeprecatedMac Catalyst 13.1–16.0DeprecatedmacOS 10.7–13.0DeprecatedtvOS 9.0–16.0Deprecated

``` source
var isReadable: Bool { get }
```

Deprecated

Load the value of isReadable asynchronously instead.

## Discussion

This property value is true if you can use AVAssetReader to extract the asset’s media data.

