

- Foundation
- NSMutableIndexSet
-  shiftIndexesStarting(at:by:) 

Instance Method

# shiftIndexesStarting(at:by:)

Shifts a group of indexes to the left or the right within the receiver.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func shiftIndexesStarting(
    at index: Int,
    by delta: Int
)
```

## Parameters 

`index`  

Head of the group of indexes to shift.

`delta`  

Amount and direction of the shift. Positive integers shift the indexes to the right. Negative integers shift the indexes to the left.

## Discussion

The group of indexes shifted is made up by `index` and the indexes that follow it in the set.

A left shift deletes the indexes in a range the length of `delta` preceding `index` from the set.

A right shift inserts empty space in the range ``` (``index``,``delta``) ``` in the receiver.

The resulting indexes must all be in the range `0 .. NSNotFound - 1`.

