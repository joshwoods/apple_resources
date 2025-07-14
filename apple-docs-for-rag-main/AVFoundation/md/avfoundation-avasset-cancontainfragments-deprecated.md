

- AVFoundation
- AVAsset
-  canContainFragments Deprecated

Instance Property

# canContainFragments

A Boolean value that indicates whether you can extend the asset by fragments.

iOS 9.0–16.0DeprecatediPadOS 9.0–16.0DeprecatedMac Catalyst 13.1–16.0DeprecatedmacOS 10.11–13.0DeprecatedtvOS 9.0–16.0Deprecated

``` source
var canContainFragments: Bool { get }
```

Deprecated

Load the value of canContainFragments asynchronously instead.

## Discussion

For QuickTime movie files and MPEG-4 files, the value is true if an `mvex` box is present in the `moov` box. For those types, the `mvex` box signals the possible presence of later `moof` boxes.

