

- AVFoundation
- AVAssetVariantQualifier
-  predicate(forAudioSampleRate:mediaSelectionOption:operatorType:) 

Type Method

# predicate(forAudioSampleRate:mediaSelectionOption:operatorType:)

Creates a predicate for audio sample rate.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
class func predicate(
    forAudioSampleRate sampleRate: Double,
    mediaSelectionOption: AVMediaSelectionOption,
    operatorType: NSComparisonPredicate.Operator
) -> NSPredicate
```

## Parameters 

`sampleRate`  

The specified sample rate to match.

`mediaSelectionOption`  

The audio media selection option under consideration.

`operatorType`  

The operator type.

## See Also

### Creating a Variant Qualifier

convenience init(variant: AVAssetVariant)

Creates a variant qualifier with an asset variant.

class AVAssetVariant

An object that represents a bit rate variant.

convenience init(predicate: NSPredicate)

Creates a variant qualifier with a predicate.

class func predicate(forChannelCount: Int, mediaSelectionOption: AVMediaSelectionOption, operatorType: NSComparisonPredicate.Operator) -> NSPredicate

Creates a predicate with a channel count, media selection option, and operator type.

class func predicate(forPresentationHeight: CGFloat, operatorType: NSComparisonPredicate.Operator) -> NSPredicate

Creates a predicate with a height and operator type.

class func predicate(forPresentationWidth: CGFloat, operatorType: NSComparisonPredicate.Operator) -> NSPredicate

Creates a predicate with a width and operator type.

class func predicate(forBinauralAudio: Bool, mediaSelectionOption: AVMediaSelectionOption) -> NSPredicate

Creates a predicate for binaural audio.

class func predicate(forDownmixAudio: Bool, mediaSelectionOption: AVMediaSelectionOption) -> NSPredicate

Creates a predicate for downmix audio.

class func predicate(forImmersiveAudio: Bool, mediaSelectionOption: AVMediaSelectionOption) -> NSPredicate

Creates a predicate for immersive audio.

