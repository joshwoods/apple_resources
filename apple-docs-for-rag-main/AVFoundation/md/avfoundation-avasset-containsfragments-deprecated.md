

- AVFoundation
- AVAsset
-  containsFragments Deprecated

Instance Property

# containsFragments

A Boolean value that indicates whether at least one movie fragment extends the asset.

iOS 9.0–16.0DeprecatediPadOS 9.0–16.0DeprecatedMac Catalyst 13.1–16.0DeprecatedmacOS 10.11–13.0DeprecatedtvOS 9.0–16.0Deprecated

``` source
var containsFragments: Bool { get }
```

Deprecated

Load the value of containsFragments asynchronously instead.

## Discussion

For QuickTime movie files and MPEG-4 files, the value is true if canContainFragments is true and at least one `moof` box is present after the `moov` box.

