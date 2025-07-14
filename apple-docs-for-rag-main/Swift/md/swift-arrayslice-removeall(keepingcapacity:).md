

- Swift
- ArraySlice
-  removeAll(keepingCapacity:) 

Instance Method

# removeAll(keepingCapacity:)

Removes all elements from the array.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
mutating func removeAll(keepingCapacity keepCapacity: Bool = false)
```

## Parameters 

`keepCapacity`  

Pass `true` to keep the existing capacity of the array after removing its elements. The default value is `false`.

## Discussion

Complexity

O(*n*), where *n* is the length of the array.

