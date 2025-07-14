

- Combine
-  ObservableObject 

Protocol

# ObservableObject

A type of object with a publisher that emits before the object has changed.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
protocol ObservableObject : AnyObject
```

## Overview

By default an ObservableObject synthesizes an objectWillChange publisher that emits the changed value before any of its `@Published` properties changes.

```
class Contact: ObservableObject {
    @Published var name: String
    @Published var age: Int

    init(name: String, age: Int) {
        self.name = name
        self.age = age
    }

    func haveBirthday() -> Int {
        age += 1
        return age
    }
}

let john = Contact(name: "John Appleseed", age: 24)
cancellable = john.objectWillChange
    .sink { _ in
        print("\(john.age) will change")
}
print(john.haveBirthday())
// Prints "24 will change"
// Prints "25"
```

## Topics

### Publishing Changes

var objectWillChange: Self.ObjectWillChangePublisher

A publisher that emits before the object has changed.

**Required** Default implementation provided.

associatedtype ObjectWillChangePublisher : Publisher = ObservableObjectPublisher

The type of publisher that emits before the object has changed.

**Required**

## See Also

### Observable Objects

class ObservableObjectPublisher

A publisher that publishes changes from observable objects.

