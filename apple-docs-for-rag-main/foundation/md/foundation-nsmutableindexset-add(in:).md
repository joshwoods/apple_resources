

- Foundation
- NSMutableIndexSet
-  add(in:) 

Instance Method

# add(in:)

Adds the indexes in an index range to the receiver.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func add(in range: NSRange)
```

## Parameters 

`range`  

Index range to add. Must be in the range `0 .. NSNotFound - 1`.

## Discussion

This method raises an rangeException when `range` would add an index that exceeds the maximum allowed value for unsigned integers.

## See Also

### Adding Indexes

func add(Int)

Adds an index to the receiver.

func add(IndexSet)

Adds the indexes in an index set to the receiver.

