

- Foundation
- NSArray
-  firstObjectCommon(with:) 

Instance Method

# firstObjectCommon(with:)

Returns the first object contained in the receiving array that’s equal to an object in another given array.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func firstObjectCommon(with otherArray: [Any]) -> Any?
```

## Parameters 

`otherArray`  

An array.

## Return Value

Returns the first object contained in the receiving array that’s equal to an object in `otherArray`. If no such object is found, returns `nil`.

## Discussion

This method uses isEqual(_:) to check for object equality.

## See Also

### Related Documentation

func contains(Any) -> Bool

Returns a Boolean value that indicates whether a given object is present in the array.

### Comparing Arrays

func isEqual(to: [Any]) -> Bool

Compares the receiving array to another array.

