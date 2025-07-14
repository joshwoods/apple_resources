

- Foundation
- IndexSet
-  insert(\_:) 

Instance Method

# insert(\_:)

Insert an integer into the `IndexSet`.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
@discardableResult
mutating func insert(_ integer: IndexSet.Element) -> (inserted: Bool, memberAfterInsert: IndexSet.Element)
```

## See Also

### Inserting Elements

func insert(integersIn: Range&lt;IndexSet.Element>)

Insert a range of integers into the `IndexSet`.

func update(with: IndexSet.Element) -> IndexSet.Element?

Insert an integer into the `IndexSet`.

