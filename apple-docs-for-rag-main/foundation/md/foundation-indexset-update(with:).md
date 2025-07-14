

- Foundation
- IndexSet
-  update(with:) 

Instance Method

# update(with:)

Insert an integer into the `IndexSet`.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
@discardableResult
mutating func update(with integer: IndexSet.Element) -> IndexSet.Element?
```

## See Also

### Inserting Elements

func insert(IndexSet.Element) -> (inserted: Bool, memberAfterInsert: IndexSet.Element)

Insert an integer into the `IndexSet`.

func insert(integersIn: Range&lt;IndexSet.Element>)

Insert a range of integers into the `IndexSet`.

