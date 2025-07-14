

- AVFoundation
- AVPlayerItemLegibleOutputPushDelegate
-  legibleOutput(\_:didOutputAttributedStrings:nativeSampleBuffers:forItemTime:) 

Instance Method

# legibleOutput(\_:didOutputAttributedStrings:nativeSampleBuffers:forItemTime:)

Asks the delegate to process the delivery of new textual samples.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+

``` source
optional func legibleOutput(
    _ output: AVPlayerItemLegibleOutput,
    didOutputAttributedStrings strings: [NSAttributedString],
    nativeSampleBuffers nativeSamples: [Any],
    forItemTime itemTime: CMTime
)
```

## Parameters 

`output`  

The AVPlayerItemLegibleOutput source instance.

`strings`  

An array of NSAttributedString objects, each containing both the run of text and the descriptive markup.

`nativeSamples`  

An array of CMSampleBuffer objects, for media subtypes included in the array passed to the `output` object’s init(mediaSubtypesForNativeRepresentation:) method.

`itemTime`  

The item time at which the strings should be presented.

## Discussion

For each media subtype in the array passed in to the `output` object’s init(mediaSubtypesForNativeRepresentation:) method, the delegate receives sample buffers carrying data in its native format via the `nativeSamples` parameter if there is media data of that subtype in the media resource.

For all other media subtypes present in the media resource, the delegate receives attributed strings in a common format via the `strings` parameter. See CMTextMarkup for the string attributes keys and values that are used in the attributed strings.

