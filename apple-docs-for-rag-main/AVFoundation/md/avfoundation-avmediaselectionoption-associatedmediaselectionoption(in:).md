

- AVFoundation
- AVMediaSelectionOption
-  associatedMediaSelectionOption(in:) 

Instance Method

# associatedMediaSelectionOption(in:)

Returns a media selection option associated with the receiver in a given group.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.8+tvOS 9.0+visionOS 1.0+watchOS 1.0+

``` source
func associatedMediaSelectionOption(in mediaSelectionGroup: AVMediaSelectionGroup) -> AVMediaSelectionOption?
```

## Parameters 

`mediaSelectionGroup`  

A media selection group in which an associated option is to be sought.

## Return Value

A media selection option associated with the receiver in `mediaSelectionGroup`, or `nil` if none were found.

## Discussion

Audible media selection options often have associated legible media selection options; in particular, audible options are typically associated with forced-only subtitle options with the same locale. See containsOnlyForcedSubtitles for a discussion of forced-only subtitles.

