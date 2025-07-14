

- AVFoundation
- AVComposition
-  canContainFragments 

Instance Property

# canContainFragments

A Boolean value that indicates whether you can extend the asset by fragments.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
var canContainFragments: Bool { get }
```

## Discussion

For QuickTime movie files and MPEG-4 files, the value is true if an `mvex` box is present in the `moov` box. For those types, the `mvex` box signals the possible presence of later `moof` boxes.

## See Also

### Determining Fragment Support

var containsFragments: Bool

A Boolean value that indicates whether at least one movie fragment extends the asset.

var overallDurationHint: CMTime

The total duration of fragments that currently exist, or may exist in the future.

