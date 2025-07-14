

- Create ML Components
- Augmenter
-  applied(to:upsampledBy:) 

Instance Method

# applied(to:upsampledBy:)

Applies an augmentation repeatedly to an array of inputs.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 11.0+

``` source
func applied(
    to elements: C,
    upsampledBy count: Int
) -> UpsampledAugmentationSequence where C : Collection, Annotation : Equatable, C.Element == AnnotatedFeature
```

## Parameters 

`elements`  

A collection of elements to augment.

`count`  

The number of times to shuffle and augment the input elements. Must be at least one.

## Return Value

A sequence of augmented elements having `count` times the number of elements in the input collection.

## Mentioned in 

Augmenting images to expand your training data

## See Also

### Applying an augmentation

func applied&lt;S, Annotation>(to: S) -> AugmentationSequence&lt;S, RandomTransformer, RandomNumberGenerator, Annotation>

Applies an augmentation per input of the base sequence.

