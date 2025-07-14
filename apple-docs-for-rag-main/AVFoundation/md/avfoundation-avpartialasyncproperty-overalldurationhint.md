

- AVFoundation
- AVPartialAsyncProperty
-  overallDurationHint 

Type Property

# overallDurationHint

A hint to the total duration of fragments that currently exist or may exist in the future.

iOS 15.0+iPadOS 15.0+Mac CatalystmacOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
static var overallDurationHint: AVAsyncProperty { get }
```

Available when `Root` inherits `AVAsset`.

## Discussion

Use the load(_:) method to retrieve the property value.

For QuickTime movie files and MPEG-4 files, the system obtains the value of this property from the `mehd` box of the `mvex` box, if present. If no total fragment duration hint is available, the value of this property is invalid.

## See Also

### Loading Fragment Support

static var canContainFragments: AVAsyncProperty&lt;Root, Bool>

A Boolean value that indicates whether you can extend the asset by fragments.

static var containsFragments: AVAsyncProperty&lt;Root, Bool>

A Boolean value that indicates whether at least one movie fragment extends the asset.

