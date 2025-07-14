

- Swift
- Slice
-  insert(contentsOf:at:) 

Instance Method

# insert(contentsOf:at:)

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
mutating func insert(
    contentsOf newElements: S,
    at i: Slice.Index
) where S : Collection, Base.Element == S.Element
```

Available when `Base` conforms to `BidirectionalCollection` and `RangeReplaceableCollection`.

