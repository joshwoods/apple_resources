

- System
- FilePath
- FilePath.ComponentView
-  removeSubrange(\_:) 

Instance Method

# removeSubrange(\_:)

Removes the elements in the specified subrange from the collection.

SystemSwiftiOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
mutating func removeSubrange(_ bounds: R) where R : RangeExpression, Self.Index == R.Bound
```

## Parameters 

`bounds`  

The range of the collection to be removed. The bounds of the range must be valid indices of the collection.

## Discussion

All the elements following the specified position are moved to close the gap. This example removes three elements from the middle of an array of measurements.

```
var measurements = [1.2, 1.5, 2.9, 1.2, 1.5]
measurements.removeSubrange(1..

Calling this method may invalidate any existing indices for use with this collection.

Complexity

O(*n*), where *n* is the length of the collection.

