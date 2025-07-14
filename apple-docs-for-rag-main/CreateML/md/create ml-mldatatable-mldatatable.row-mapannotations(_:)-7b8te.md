

- Create ML
- MLDataTable
- MLDataTable.Row
-  mapAnnotations(\_:) 

Instance Method

# mapAnnotations(\_:)

Returns an array containing the results of mapping the given closure over the sequence’s annotations.

Create MLSwiftiOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 11.0+

``` source
func mapAnnotations(_ transform: (Input) throws -> Output) rethrows -> [AnnotatedFeature] where Self.Element == AnnotatedFeature
```

