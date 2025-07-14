

- AVFoundation
- AVPartialAsyncProperty
-  canContainFragments 

Type Property

# canContainFragments

A Boolean value that indicates whether you can extend the asset by fragments.

iOS 15.0+iPadOS 15.0+Mac CatalystmacOS 12.0+tvOS 15.0+visionOS 1.0+

``` source
static var canContainFragments: AVAsyncProperty { get }
```

Available when `Root` inherits `AVAsset`.

## Discussion

Use the load(_:) method to retrieve the property value.

For QuickTime movie files and MPEG-4 files, the value is true if an `mvex` box is present in the `moov` box. For those types, the `mvex` box signals the possible presence of later `moof` boxes.

## See Also

### Loading Fragment Support

static var containsFragments: AVAsyncProperty&lt;Root, Bool>

A Boolean value that indicates whether at least one movie fragment extends the asset.

static var overallDurationHint: AVAsyncProperty&lt;Root, CMTime>

A hint to the total duration of fragments that currently exist or may exist in the future.

