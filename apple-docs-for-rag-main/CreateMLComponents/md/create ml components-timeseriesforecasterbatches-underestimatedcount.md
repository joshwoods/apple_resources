

- Create ML Components
- TimeSeriesForecasterBatches
-  underestimatedCount 

Instance Property

# underestimatedCount

A value less than or equal to the number of elements in the sequence, calculated nondestructively.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
var underestimatedCount: Int { get }
```

## Discussion

The default implementation returns 0. If you provide your own implementation, make sure to compute the value nondestructively.

Complexity

O(1), except if the sequence also conforms to `Collection`. In this case, see the documentation of `Collection.underestimatedCount`.

