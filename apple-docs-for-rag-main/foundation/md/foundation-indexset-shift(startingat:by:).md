

- Foundation
- IndexSet
-  shift(startingAt:by:) 

Instance Method

# shift(startingAt:by:)

For a positive delta, shifts the indexes in \[index, INT_MAX\] to the right, thereby inserting an “empty space” \[index, delta\], for a negative delta, shifts the indexes in \[index, INT_MAX\] to the left, thereby deleting the indexes in the range \[index - delta, delta\].

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
mutating func shift(
    startingAt integer: IndexSet.Element,
    by delta: Int
)
```

