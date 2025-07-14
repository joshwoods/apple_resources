

- RoomPlan
- CapturedRoom
- CapturedRoom.Surface
- CapturedRoom.Surface.Edge
-  hashValue 

Instance Property

# hashValue

The hash value.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+

``` source
var hashValue: Int { get }
```

## Discussion

Hash values are not guaranteed to be equal across different executions of your program. Do not save hash values to use during a future execution.

Important

`hashValue` is deprecated as a `Hashable` requirement. To conform to `Hashable`, implement the `hash(into:)` requirement instead. The compiler provides an implementation for `hashValue` for you.

## See Also

### Comparing edges

static func == (CapturedRoom.Surface.Edge, CapturedRoom.Surface.Edge) -> Bool

Determines whether two surface edges are equal.

static func != (Self, Self) -> Bool

Determines whether two surface edges aren’t equal.

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

