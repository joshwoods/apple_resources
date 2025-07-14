

- Foundation
- NSArray
-  isEqual(to:) 

Instance Method

# isEqual(to:)

Compares the receiving array to another array.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func isEqual(to otherArray: [Any]) -> Bool
```

## Parameters 

`otherArray`  

An array.

## Return Value

true if the contents of `otherArray` are equal to the contents of the receiving array, otherwise false.

## Discussion

Two arrays have equal contents if they each hold the same number of objects and objects at a given index in each array satisfy the isEqual(_:) test.

## See Also

### Comparing Arrays

func firstObjectCommon(with: [Any]) -> Any?

Returns the first object contained in the receiving array that’s equal to an object in another given array.

