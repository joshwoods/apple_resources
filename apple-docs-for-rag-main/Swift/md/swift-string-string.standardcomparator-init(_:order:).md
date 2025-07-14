

- Swift
- String
- String.StandardComparator
-  init(\_:order:) 

Initializer

# init(\_:order:)

Create a `StandardComparator` from the given `StandardComparator` with the given new `order`.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
init(
    _ base: String.StandardComparator,
    order: SortOrder = .forward
)
```

## Parameters 

`base`  

The standard comparator to modify the order of.

`order`  

The initial order of the new `StandardComparator`.

