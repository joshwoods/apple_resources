

- AVFoundation
- AVPartialAsyncProperty
-  containsFragments 

Type Property

# containsFragments

A Boolean value that indicates whether at least one movie fragment extends the asset.

iOS 15.0+iPadOS 15.0+Mac CatalystmacOS 12.0+tvOS 15.0+visionOS 1.0+

``` source
static var containsFragments: AVAsyncProperty { get }
```

Available when `Root` inherits `AVAsset`.

## Discussion

Use the load(_:) method to retrieve the property value.

For QuickTime movie files and MPEG-4 files, the value of this property is true if canContainFragments is true and at least one `moof` box is present after the `moov` box.

## See Also

### Loading Fragment Support

static var canContainFragments: AVAsyncProperty&lt;Root, Bool>

A Boolean value that indicates whether you can extend the asset by fragments.

static var overallDurationHint: AVAsyncProperty&lt;Root, CMTime>

A hint to the total duration of fragments that currently exist or may exist in the future.

