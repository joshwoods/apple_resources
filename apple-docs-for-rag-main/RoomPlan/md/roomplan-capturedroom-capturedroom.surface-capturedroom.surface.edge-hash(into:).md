

- RoomPlan
- CapturedRoom
- CapturedRoom.Surface
- CapturedRoom.Surface.Edge
-  hash(into:) 

Instance Method

# hash(into:)

Hashes the essential components of this value by feeding them into the given hasher.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+

``` source
func hash(into hasher: inout Hasher)
```

## Parameters 

`hasher`  

The hasher to use when combining the components of this instance.

## Discussion

Implement this method to conform to the `Hashable` protocol. The components used for hashing must be the same as the components compared in your type’s `==` operator implementation. Call `hasher.combine(_:)` with each of these components.

Important

In your implementation of `hash(into:)`, don’t call `finalize()` on the `hasher` instance provided, or replace it with a different instance. Doing so may become a compile-time error in the future.

## See Also

### Comparing edges

static func == (CapturedRoom.Surface.Edge, CapturedRoom.Surface.Edge) -> Bool

Determines whether two surface edges are equal.

static func != (Self, Self) -> Bool

Determines whether two surface edges aren’t equal.

var hashValue: Int

The hash value.

