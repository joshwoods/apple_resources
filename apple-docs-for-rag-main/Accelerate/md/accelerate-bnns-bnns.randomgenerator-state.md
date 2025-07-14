

- Accelerate
- BNNS
- BNNS.RandomGenerator
-  state 

Instance Property

# state

The state of the random number generator.

iOS 15.0+iPadOS 15.0+Mac CatalystmacOS 12.0+tvOS 15.0+visionOSwatchOS 8.0+

``` source
var state: BNNS.RandomGeneratorState { get set }
```

## Discussion

Use the random number generator’s state property to save and restore the generator.

The following code creates a random number generator and captures its initial state. The code calls allocate(randomUniformUsing:range:shape:batchSize:) twice to populate the arrays `a` and `b` with different random values. Before allocating the array `c` with random values, the code resets the generator’s state to create identical random values in arrays `a` and `c`.

```
guard
    let randomGenerator = BNNS.RandomGenerator(
        method: .aesCtr,
        seed: 1234) else {
        return
    }

let state = randomGenerator.state

let a = BNNSNDArrayDescriptor.allocate(
    randomUniformUsing: randomGenerator,
    range: Int16(-10)...Int16(10),
    shape: [16])!.makeArray(of: Int16.self)!

let b = BNNSNDArrayDescriptor.allocate(
    randomUniformUsing: randomGenerator,
    range: Int16(-10)...Int16(10),
    shape: [16])!.makeArray(of: Int16.self)!

// Prints "false".
print(a.elementsEqual(b))

randomGenerator.state = state

let c = BNNSNDArrayDescriptor.allocate(
    randomUniformUsing: randomGenerator,
    range: Int16(-10)...Int16(10),
    shape: [16])!.makeArray(of: Int16.self)!

// Prints "true".
print(a.elementsEqual(c))
```

## See Also

### Saving and Restoring a Randon Generator’s State

class RandomGeneratorState

An opaque object that contains the state of a random number generator.

