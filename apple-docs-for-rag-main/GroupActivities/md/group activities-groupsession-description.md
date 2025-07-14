

- Group Activities
- GroupSession
-  description 

Instance Property

# description

A textual representation of this instance.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+

``` source
final var description: String { get }
```

Available when `ActivityType` conforms to `GroupActivity`.

## Discussion

Calling this property directly is discouraged. Instead, convert an instance of any type to a string by using the `String(describing:)` initializer. This initializer works with any type, and uses the custom `description` property for types that conform to `CustomStringConvertible`:

```
struct Point: CustomStringConvertible {
    let x: Int, y: Int

    var description: String {
        return "(\(x), \(y))"
    }
}

let p = Point(x: 21, y: 30)
let s = String(describing: p)
print(s)
// Prints "(21, 30)"
```

The conversion of `p` to a string in the assignment to `s` uses the `Point` type’s `description` property.

## See Also

### Getting the session details

var state: GroupSession&lt;ActivityType>.State

The current state of the session.

enum State

The possible states of a session.

let id: UUID

The unique identifier of the current session.

