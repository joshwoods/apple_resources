

- Swift
- Set
-  update(with:) 

Instance Method

# update(with:)

Inserts the given element into the set unconditionally.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
@discardableResult
mutating func update(with newMember: Element) -> Element?
```

Available when `Element` conforms to `Hashable`.

## Parameters 

`newMember`  

An element to insert into the set.

## Return Value

An element equal to `newMember` if the set already contained such a member; otherwise, `nil`. In some cases, the returned element may be distinguishable from `newMember` by identity comparison or some other means.

## Discussion

If an element equal to `newMember` is already contained in the set, `newMember` replaces the existing element. In this example, an existing element is inserted into `classDays`, a set of days of the week.

```
enum DayOfTheWeek: Int {
    case sunday, monday, tuesday, wednesday, thursday,
        friday, saturday
}

var classDays: Set = [.monday, .wednesday, .friday]
print(classDays.update(with: .monday))
// Prints "Optional(DayOfTheWeek.monday)"
```

## See Also

### Adding Elements

func insert(Element) -> (inserted: Bool, memberAfterInsert: Element)

Inserts the given element in the set if it is not already present.

func insert&lt;ConcreteElement>(ConcreteElement) -> (inserted: Bool, memberAfterInsert: ConcreteElement)

func update&lt;ConcreteElement>(with: ConcreteElement) -> ConcreteElement?

func reserveCapacity(Int)

Reserves enough space to store the specified number of elements.

