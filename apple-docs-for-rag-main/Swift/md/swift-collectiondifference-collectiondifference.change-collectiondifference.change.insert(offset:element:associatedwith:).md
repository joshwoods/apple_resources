

- Swift
- CollectionDifference
- CollectionDifference.Change
-  CollectionDifference.Change.insert(offset:element:associatedWith:) 

Case

# CollectionDifference.Change.insert(offset:element:associatedWith:)

An insertion.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
case insert(
    offset: Int,
    element: ChangeElement,
    associatedWith: Int?
)
```

## Discussion

The `offset` value is the offset of the inserted element in the final state of the collection after the difference is fully applied. A non-`nil` `associatedWith` value is the offset of the complementary change.

