

- Create ML
- MLSoundClassifier
- MLSoundClassifier.ModelParameters
- MLSoundClassifier.ModelParameters.FeatureExtractorType
-  MLSoundClassifier.ModelParameters.FeatureExtractorType.vggish(revision:) 

Case

# MLSoundClassifier.ModelParameters.FeatureExtractorType.vggish(revision:)

Represents the VGGish feature extractor, which is compatible with older OS versions.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 11.0+visionOS 1.0+

``` source
case vggish(revision: Int = 1)
```

## Parameters 

`revision`  

A version of the VGGish feature extractor.

## Discussion

The case uses the newest version if you don’t provide an associated value for `revision`.

## See Also

### Designating a feature extractor

case audioFeaturePrint(type: MLSoundClassifier.ModelParameters.FeaturePrintType, revision: Int)

Represents the Audio Feature Print extractor.

enum FeaturePrintType

The type options for an Audio Feature Print feature extractor.

