

- Create ML Components
- TimeSeriesForecasterAnnotatedWindows
-  TimeSeriesForecasterAnnotatedWindows.Iterator 

Structure

# TimeSeriesForecasterAnnotatedWindows.Iterator

A time-series forecaster batch sequence iterator.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
struct Iterator
```

Available when `Scalar` conforms to `MLShapedArrayScalar`.

## Topics

### Instance Methods

func next() -> AnnotatedFeature&lt;MLShapedArray&lt;Scalar>, MLShapedArray&lt;Scalar>>?

Advances to the next element and returns it, or `nil` if no next element exists.

### Type Aliases

typealias Element

The type of element traversed by the iterator.

## Relationships

### Conforms To

- IteratorProtocol
- Sendable

