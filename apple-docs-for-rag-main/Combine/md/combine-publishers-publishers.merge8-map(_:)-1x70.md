

- Combine
- Publishers
- Publishers.Merge8
-  map(\_:) 

Instance Method

# map(\_:)

Publishes the value of a key path.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
func map(_ keyPath: KeyPath) -> Publishers.MapKeyPath
```

## Parameters 

`keyPath`  

The key path of a property on `Output`.

## Return Value

A publisher that publishes the value of the key path.

## Discussion

In the following example, the map(_:) operator uses the Swift key path syntax to access the `die` member of the `DiceRoll` structure published by the Just publisher.

The downstream sink subscriber receives only the value of this `Int`, not the entire `DiceRoll`.

```
struct DiceRoll {
    let die: Int
}

cancellable = Just(DiceRoll(die:Int.random(in:1...6)))
    .map(\.die)
    .sink {
        print ("Rolled: \($0)")
    }
// Prints "Rolled: 3" (or some other random value).
```

## See Also

### Identifying Properties with Key Paths

func map&lt;T0, T1>(KeyPath&lt;Self.Output, T0>, KeyPath&lt;Self.Output, T1>) -> Publishers.MapKeyPath2&lt;Self, T0, T1>

Publishes the values of two key paths as a tuple.

func map&lt;T0, T1, T2>(KeyPath&lt;Self.Output, T0>, KeyPath&lt;Self.Output, T1>, KeyPath&lt;Self.Output, T2>) -> Publishers.MapKeyPath3&lt;Self, T0, T1, T2>

Publishes the values of three key paths as a tuple.

