

- Foundation
- NSArray
-  addingObjects(from:) 

Instance Method

# addingObjects(from:)

Returns a new array that is a copy of the receiving array with the objects contained in another array added to the end.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func addingObjects(from otherArray: [Any]) -> [Any]
```

## Parameters 

`otherArray`  

An array.

## Return Value

A new array that is a copy of the receiving array with the objects contained in `otherArray` added to the end.

## See Also

### Related Documentation

func addObjects(from: [Any])

Adds the objects contained in another given array to the end of the receiving array’s content.

### Deriving New Arrays

func adding(Any) -> [Any]

Returns a new array that is a copy of the receiving array with a given object added to the end.

func filtered(using: NSPredicate) -> [Any]

Evaluates a given predicate against each object in the receiving array and returns a new array containing the objects for which the predicate returns true.

func subarray(with: NSRange) -> [Any]

Returns a new array containing the receiving array’s elements that fall within the limits specified by a given range.

