

- RealityKit
- LoadRequest
-  map(\_:\_:) 

Instance Method

# map(\_:\_:)

Publishes the values of two key paths as a tuple.

RealityKitCombineiOS 13.0+iPadOS 13.0+Mac CatalystmacOS 10.15+tvOS 13.0+visionOSwatchOS 6.0+

``` source
func map(
    _ keyPath0: KeyPath,
    _ keyPath1: KeyPath
) -> Publishers.MapKeyPath2
```

## Parameters 

`keyPath0`  

The key path of a property on `Output`.

`keyPath1`  

The key path of another property on `Output`.

## Return Value

A publisher that publishes the values of two key paths as a tuple.

## Discussion

In the following example, the `Publisher/map(_:_:)` operator uses the Swift key path syntax to access the `die1` and `die2` members of the `DiceRoll` structure published by the `Just` publisher.

The downstream sink subscriber receives only these two values (as an `(Int, Int)` tuple), not the entire `DiceRoll`.

```
struct DiceRoll {
    let die1: Int
    let die2: Int
}

cancellable = Just(DiceRoll(die1:Int.random(in:1...6),
                            die2: Int.random(in:1...6)))
    .map(\.die1, \.die2)
    .sink { values in
        print ("Rolled: \(values.0), \(values.1) (total: \(values.0 + values.1))")
    }
// Prints "Rolled: 6, 4 (total: 10)" (or other random values).
```

## See Also

### Identifying properties with key paths

func map&lt;T>(KeyPath&lt;Self.Output, T>) -> Publishers.MapKeyPath&lt;Self, T>

Publishes the value of a key path.

func map&lt;T0, T1, T2>(KeyPath&lt;Self.Output, T0>, KeyPath&lt;Self.Output, T1>, KeyPath&lt;Self.Output, T2>) -> Publishers.MapKeyPath3&lt;Self, T0, T1, T2>

Publishes the values of three key paths as a tuple.

