

- Create ML Components
- Augmenter
-  applied(to:) 

Instance Method

# applied(to:)

Applies an augmentation per input of the base sequence.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 11.0+

``` source
func applied(to base: S) -> AugmentationSequence where S : Sequence, Annotation : Equatable, S.Element == AnnotatedFeature
```

## Parameters 

`base`  

A sequence of elements to augment.

## Return Value

A sequence of augmented elements having the same number of elements as the input sequence.

## Mentioned in 

Augmenting images to expand your training data

## See Also

### Applying an augmentation

func applied&lt;C, Annotation>(to: C, upsampledBy: Int) -> UpsampledAugmentationSequence&lt;C, RandomTransformer, RandomNumberGenerator, Annotation>

Applies an augmentation repeatedly to an array of inputs.

