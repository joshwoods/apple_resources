

- Swift
- Optional
- Optional.Publisher
-  map(\_:) 

Instance Method

# map(\_:)

Publishes the value of a key path.

SwiftCombineiOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
func map(_ keyPath: KeyPath) -> Publishers.MapKeyPath
```

## Parameters 

`keyPath`  

The key path of a property on `Output`.

## Return Value

A publisher that publishes the value of the key path.

## Discussion

In the following example, the `Publisher/map(_:)-6sm0a` operator uses the Swift key path syntax to access the `die` member of the `DiceRoll` structure published by the `Just` publisher.

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

