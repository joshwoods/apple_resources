

- TabularData
- DiscontiguousColumnSlice
-  firstIndex(of:) 

Instance Method

# firstIndex(of:)

Returns the first index where the specified value appears in the collection.

TabularDataSwiftiOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
func firstIndex(of element: Self.Element) -> Self.Index?
```

Available when `Element` conforms to `Equatable`.

## Parameters 

`element`  

An element to search for in the collection.

## Return Value

The first index where `element` is found. If `element` is not found in the collection, returns `nil`.

## Discussion

After using `firstIndex(of:)` to find the position of a particular element in a collection, you can use it to access the element by subscripting. This example shows how you can modify one of the names in an array of students.

```
var students = ["Ben", "Ivy", "Jordell", "Maxime"]
if let i = students.firstIndex(of: "Maxime") {
    students[i] = "Max"
}
print(students)
// Prints "["Ben", "Ivy", "Jordell", "Max"]"
```

Complexity

O(*n*), where *n* is the length of the collection.

