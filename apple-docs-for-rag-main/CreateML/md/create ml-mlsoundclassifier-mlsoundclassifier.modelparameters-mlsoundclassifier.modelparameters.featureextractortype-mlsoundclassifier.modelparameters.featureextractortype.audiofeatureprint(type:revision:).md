

- Create ML
- MLSoundClassifier
- MLSoundClassifier.ModelParameters
- MLSoundClassifier.ModelParameters.FeatureExtractorType
-  MLSoundClassifier.ModelParameters.FeatureExtractorType.audioFeaturePrint(type:revision:) 

Case

# MLSoundClassifier.ModelParameters.FeatureExtractorType.audioFeaturePrint(type:revision:)

Represents the Audio Feature Print extractor.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS 1.0+

``` source
case audioFeaturePrint(
    type: MLSoundClassifier.ModelParameters.FeaturePrintType = .sound,
    revision: Int = 1
)
```

## Parameters 

`type`  

An Audio Feature Print extractor type.

`revision`  

A version of the extractor you pass to `type`.

## Discussion

The case uses the newest version of MLSoundClassifier.ModelParameters.FeaturePrintType.sound if you don’t provide associated values for `type` and `revision`.

## See Also

### Designating a feature extractor

enum FeaturePrintType

The type options for an Audio Feature Print feature extractor.

case vggish(revision: Int)

Represents the VGGish feature extractor, which is compatible with older OS versions.

