

- AVFoundation
- AVComposition
-  containsFragments 

Instance Property

# containsFragments

A Boolean value that indicates whether at least one movie fragment extends the asset.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
var containsFragments: Bool { get }
```

## Discussion

For QuickTime movie files and MPEG-4 files, the value is true if canContainFragments is true and at least one `moof` box is present after the `moov` box.

## See Also

### Determining Fragment Support

var canContainFragments: Bool

A Boolean value that indicates whether you can extend the asset by fragments.

var overallDurationHint: CMTime

The total duration of fragments that currently exist, or may exist in the future.

