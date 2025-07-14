

- Swift
- Set
-  reserveCapacity(\_:) 

Instance Method

# reserveCapacity(\_:)

Reserves enough space to store the specified number of elements.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
mutating func reserveCapacity(_ minimumCapacity: Int)
```

Available when `Element` conforms to `Hashable`.

## Parameters 

`minimumCapacity`  

The requested number of elements to store.

## Discussion

If you are adding a known number of elements to a set, use this method to avoid multiple reallocations. This method ensures that the set has unique, mutable, contiguous storage, with space allocated for at least the requested number of elements.

Calling the `reserveCapacity(_:)` method on a set with bridged storage triggers a copy to contiguous storage even if the existing storage has room to store `minimumCapacity` elements.

## See Also

### Adding Elements

func insert(Element) -> (inserted: Bool, memberAfterInsert: Element)

Inserts the given element in the set if it is not already present.

func insert&lt;ConcreteElement>(ConcreteElement) -> (inserted: Bool, memberAfterInsert: ConcreteElement)

func update(with: Element) -> Element?

Inserts the given element into the set unconditionally.

func update&lt;ConcreteElement>(with: ConcreteElement) -> ConcreteElement?

