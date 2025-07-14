

- Swift
- Set
-  insert(\_:) 

Instance Method

# insert(\_:)

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
@discardableResult
mutating func insert(_ newMember: ConcreteElement) -> (inserted: Bool, memberAfterInsert: ConcreteElement) where ConcreteElement : Hashable
```

Available when `Element` is `AnyHashable`.

## See Also

### Adding Elements

func insert(Element) -> (inserted: Bool, memberAfterInsert: Element)

Inserts the given element in the set if it is not already present.

func update(with: Element) -> Element?

Inserts the given element into the set unconditionally.

func update&lt;ConcreteElement>(with: ConcreteElement) -> ConcreteElement?

func reserveCapacity(Int)

Reserves enough space to store the specified number of elements.

