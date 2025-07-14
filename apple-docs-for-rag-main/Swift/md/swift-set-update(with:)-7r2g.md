

- Swift
- Set
-  update(with:) 

Instance Method

# update(with:)

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
@discardableResult
mutating func update(with newMember: ConcreteElement) -> ConcreteElement? where ConcreteElement : Hashable
```

Available when `Element` is `AnyHashable`.

## See Also

### Adding Elements

func insert(Element) -> (inserted: Bool, memberAfterInsert: Element)

Inserts the given element in the set if it is not already present.

func insert&lt;ConcreteElement>(ConcreteElement) -> (inserted: Bool, memberAfterInsert: ConcreteElement)

func update(with: Element) -> Element?

Inserts the given element into the set unconditionally.

func reserveCapacity(Int)

Reserves enough space to store the specified number of elements.

