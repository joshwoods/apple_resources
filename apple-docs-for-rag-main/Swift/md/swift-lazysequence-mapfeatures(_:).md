

- Swift
- LazySequence
-  mapFeatures(\_:) 

Instance Method

# mapFeatures(\_:)

Returns a lazy sequence where the elements of the result are computed each time they are read by calling transform function on the feature of an annotated feature.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 11.0+

``` source
func mapFeatures(_ transform: @escaping (Input) -> Output) -> LazyMapSequence> where Base.Element == AnnotatedFeature
```

Available when `Base` conforms to `Sequence`.

