

- Swift
- CollectionDifference
- CollectionDifference.Change
-  CollectionDifference.Change.remove(offset:element:associatedWith:) 

Case

# CollectionDifference.Change.remove(offset:element:associatedWith:)

A removal.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
case remove(
    offset: Int,
    element: ChangeElement,
    associatedWith: Int?
)
```

## Discussion

The `offset` value is the offset of the element to be removed in the original state of the collection. A non-`nil` `associatedWith` value is the offset of the complementary change.

