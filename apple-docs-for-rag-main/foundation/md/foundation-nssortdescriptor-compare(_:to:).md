

- Foundation
- NSSortDescriptor
-  compare(\_:to:) 

Instance Method

# compare(\_:to:)

Returns a comparison result value that indicates the sort order of two objects.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func compare(
    _ object1: Any,
    to object2: Any
) -> ComparisonResult
```

## Parameters 

`object1`  

The object to compare with `object2`. This object must have a property accessible using the key-path specified by key.

`object2`  

The object to compare with `object1`. This object must have a property accessible using the key-path specified by key.

## Return Value

ComparisonResult.orderedAscending if `object1` is less than `object2`, ComparisonResult.orderedDescending if `object1` is greater than `object2`, or ComparisonResult.orderedSame if `object1` is equal to `object2`.

## Discussion

The ordering is determined by comparing the values specified by key of `object1` and `object2` using the selector specified by selector.

## See Also

### Using Sort Descriptors

var reversedSortDescriptor: Any

Returns a sort descriptor that reverses the sort order.

func allowEvaluation()

Forces a securely decoded sort descriptor to allow evaluation.

