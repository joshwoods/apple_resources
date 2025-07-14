

- Create ML Components
- SlidingWindows
-  mapFeatures(\_:) 

Instance Method

# mapFeatures(\_:)

Returns an array containing the results of mapping the given closure over the sequence’s features.

Create ML ComponentsSwiftiOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 11.0+

``` source
func mapFeatures(_ transform: (Input) throws -> Output) rethrows -> [AnnotatedFeature] where Self.Element == AnnotatedFeature
```

