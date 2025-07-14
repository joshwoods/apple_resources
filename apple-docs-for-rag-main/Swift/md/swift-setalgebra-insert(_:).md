

- Swift
- SetAlgebra
-  insert(\_:) 

Instance Method

# insert(\_:)

Inserts the given element in the set if it is not already present.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
@discardableResult
mutating func insert(_ newMember: Self.Element) -> (inserted: Bool, memberAfterInsert: Self.Element)
```

**Required** Default implementation provided.

## Parameters 

`newMember`  

An element to insert into the set.

## Return Value

`(true, newMember)` if `newMember` was not contained in the set. If an element equal to `newMember` was already contained in the set, the method returns `(false, oldMember)`, where `oldMember` is the element that was equal to `newMember`. In some cases, `oldMember` may be distinguishable from `newMember` by identity comparison or some other means.

## Discussion

If an element equal to `newMember` is already contained in the set, this method has no effect. In this example, a new element is inserted into `classDays`, a set of days of the week. When an existing element is inserted, the `classDays` set does not change.

```
enum DayOfTheWeek: Int {
    case sunday, monday, tuesday, wednesday, thursday,
        friday, saturday
}

var classDays: Set = [.wednesday, .friday]
print(classDays.insert(.monday))
// Prints "(true, .monday)"
print(classDays)
// Prints "[.friday, .wednesday, .monday]"

print(classDays.insert(.friday))
// Prints "(false, .friday)"
print(classDays)
// Prints "[.friday, .wednesday, .monday]"
```

## Default Implementations

### SetAlgebra Implementations

func insert(Self.Element) -> (inserted: Bool, memberAfterInsert: Self.Element)

Adds the given element to the option set if it is not already a member.

## See Also

### Adding and Removing Elements

func update(with: Self.Element) -> Self.Element?

Inserts the given element into the set unconditionally.

**Required** Default implementation provided.

func remove(Self.Element) -> Self.Element?

Removes the given element and any elements subsumed by the given element.

**Required** Default implementation provided.

