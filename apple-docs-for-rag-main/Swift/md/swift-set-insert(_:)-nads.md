

- Swift
- Set
-  insert(\_:) 

Instance Method

# insert(\_:)

Inserts the given element in the set if it is not already present.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
@discardableResult
mutating func insert(_ newMember: Element) -> (inserted: Bool, memberAfterInsert: Element)
```

Available when `Element` conforms to `Hashable`.

## Parameters 

`newMember`  

An element to insert into the set.

## Return Value

`(true, newMember)` if `newMember` was not contained in the set. If an element equal to `newMember` was already contained in the set, the method returns `(false, oldMember)`, where `oldMember` is the element that was equal to `newMember`. In some cases, `oldMember` may be distinguishable from `newMember` by identity comparison or some other means.

## Discussion

If an element equal to `newMember` is already contained in the set, this method has no effect. In the following example, a new element is inserted into `classDays`, a set of days of the week. When an existing element is inserted, the `classDays` set does not change.

```
enum DayOfTheWeek: Int {
    case sunday, monday, tuesday, wednesday, thursday,
        friday, saturday
}

var classDays: Set = [.wednesday, .friday]
print(classDays.insert(.monday))
// Prints "(inserted: true, memberAfterInsert: DayOfTheWeek.monday)"
print(classDays)
// Prints "[DayOfTheWeek.friday, DayOfTheWeek.wednesday, DayOfTheWeek.monday]"

print(classDays.insert(.friday))
// Prints "(inserted: false, memberAfterInsert: DayOfTheWeek.friday)"
print(classDays)
// Prints "[DayOfTheWeek.friday, DayOfTheWeek.wednesday, DayOfTheWeek.monday]"
```

## See Also

### Adding Elements

func insert&lt;ConcreteElement>(ConcreteElement) -> (inserted: Bool, memberAfterInsert: ConcreteElement)

func update(with: Element) -> Element?

Inserts the given element into the set unconditionally.

func update&lt;ConcreteElement>(with: ConcreteElement) -> ConcreteElement?

func reserveCapacity(Int)

Reserves enough space to store the specified number of elements.

