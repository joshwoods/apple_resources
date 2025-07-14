

- AVFoundation
- AVAssetVariantQualifier
-  predicate(forImmersiveAudio:mediaSelectionOption:) 

Type Method

# predicate(forImmersiveAudio:mediaSelectionOption:)

Creates a predicate for immersive audio.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
class func predicate(
    forImmersiveAudio isImmersiveAudio: Bool,
    mediaSelectionOption: AVMediaSelectionOption
) -> NSPredicate
```

## Parameters 

`isImmersiveAudio`  

`mediaSelectionOption`  

The media selection option for the variant.

## Return Value

A predicate object that you use to to create an AVAssetVariantQualifier.

## Discussion

Use the returned value, along with other predicates, to express variant preferences.

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

class func predicate(forAudioSampleRate: Double, mediaSelectionOption: AVMediaSelectionOption, operatorType: NSComparisonPredicate.Operator) -> NSPredicate

Creates a predicate for audio sample rate.

