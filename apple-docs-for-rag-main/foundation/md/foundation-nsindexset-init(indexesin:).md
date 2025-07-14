

- Foundation
- NSIndexSet
-  init(indexesIn:) 

Initializer

# init(indexesIn:)

Initializes an allocated NSIndexSet object with an index range.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
init(indexesIn range: NSRange)
```

## Parameters 

`range`  

An index range. Must be in the range `0 .. NSNotFound - 1`..

## Return Value

Initialized NSIndexSet object with `indexRange`.

## Discussion

This method raises an rangeException when `indexRange` would add an index that exceeds the maximum allowed value for unsigned integers.

The resulting index set has a firstIndex equal to the `location` of `indexRange`, and a count equal to the `length` of `indexRange`. Specifying a zero-length range results in an empty index set.

This method is a designated initializer for NSIndexSet.

## See Also

### Creating Index Sets

convenience init(index: Int)

Initializes an allocated NSIndexSet object with an index.

init(indexSet: IndexSet)

Initializes an allocated NSIndexSet object with an index set.

