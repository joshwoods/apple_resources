

- Create ML
-  MLStreamingVisualizable 

Protocol

# MLStreamingVisualizable

A sequence of image visualizations for machine learning types.

macOS 10.15+

``` source
protocol MLStreamingVisualizable : MLVisualizable
```

## Topics

### Seeing the next visualization

var hasFinishedStreaming: Bool

A Boolean value that indicates whether the stream has provided its final iteration.

**Required**

func nextIteration()

Advances the visualization stream to the next iteration.

**Required**

## Relationships

### Inherits From

- CustomPlaygroundDisplayConvertible
- MLVisualizable

## See Also

### Visualization Protocols

protocol MLVisualizable

An image visualization of machine learning types.

