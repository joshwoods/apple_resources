

- Accelerate
-  BNNSRandomGeneratorSetState(\_:\_:\_:) 

Function

# BNNSRandomGeneratorSetState(\_:\_:\_:)

Sets the state of a random number generator.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
func BNNSRandomGeneratorSetState(
    _ generator: BNNSRandomGenerator?,
    _ state_size: Int,
    _ state: UnsafeMutableRawPointer
) -> Int32
```

## Parameters 

`generator`  

The random number generator.

`state_size`  

The size of the state buffer, in bytes.

`state`  

A pointer to the state.

## Discussion

Use the BNNSRandomGeneratorGetState(_:_:_:) and BNNSRandomGeneratorSetState(_:_:_:) functions to capture and restore a random number generator’s state.

The following code creates a random number generator and captures its initial state. The code calls BNNSRandomFillUniformInt(_:_:_:_:) twice and copies the random values into the arrays `a` and `b`. The BNNSRandomGeneratorSetState(_:_:_:) function restores the generator to its initial state, and the final call to BNNSRandomFillUniformInt(_:_:_:_:) populates the descriptor so that the values in arrays `a` and `c` are equal.

```
let data = UnsafeMutableBufferPointer.allocate(capacity: 8)
var descriptor = BNNSNDArrayDescriptor(flags: BNNSNDArrayFlags(0),
                                       layout: BNNSDataLayoutVector,
                                       size: (10, 0, 0, 0, 0, 0, 0, 0),
                                       stride: (0, 0, 0, 0, 0, 0, 0, 0),
                                       data: data.baseAddress!,
                                       data_type: BNNSDataType.int16,
                                       table_data: nil,
                                       table_data_type: BNNSDataType.int16,
                                       data_scale: 1, data_bias: 0)

guard let randomNumberGenerator = BNNSCreateRandomGenerator(BNNSRandomGeneratorMethodAES_CTR,
                                                            nil) else {
    return
}

// Allocate memory to store state.
let stateSize = BNNSRandomGeneratorStateSize(randomNumberGenerator)
let state = UnsafeMutableRawPointer.allocate(byteCount: stateSize,
                                             alignment: 0)

// Store the random number generator's state.
BNNSRandomGeneratorGetState(randomNumberGenerator,
                            stateSize,
                            state)

BNNSRandomFillUniformInt(randomNumberGenerator,
                         &descriptor,
                         -10,
                         10)

let a = Array(data)

BNNSRandomFillUniformInt(randomNumberGenerator,
                         &descriptor,
                         -10,
                         10)

let b = Array(data)

// Set the random number generator's state to its initial state.
BNNSRandomGeneratorSetState(randomNumberGenerator,
                            stateSize,
                            state)

BNNSRandomFillUniformInt(randomNumberGenerator,
                         &descriptor,
                         -10,
                         10)

let c = Array(data)

print(a.elementsEqual(c)) // prints "true"

data.deallocate()
state.deallocate()
BNNSDestroyRandomGenerator(randomNumberGenerator)
```

## See Also

### Random number generation

class RandomGenerator

A random number generator.

func BNNSCreateRandomGenerator(BNNSRandomGeneratorMethod, UnsafePointer&lt;BNNSFilterParameters>?) -> BNNSRandomGenerator?

Returns a new random number generator using an internally generated random seed.

func BNNSCreateRandomGeneratorWithSeed(BNNSRandomGeneratorMethod, UInt64, UnsafePointer&lt;BNNSFilterParameters>?) -> BNNSRandomGenerator?

Returns a new random number generator using the specified seed.

struct BNNSRandomGeneratorMethod

Constants that describe random number generation methods.

typealias BNNSRandomGenerator

A pointer to a random number generator object.

func BNNSRandomFillUniformInt(BNNSRandomGenerator?, UnsafeMutablePointer&lt;BNNSNDArrayDescriptor>, Int64, Int64) -> Int32

Fills the specified tensor with random integer values from the continuous uniform distribution within a range.

func BNNSRandomFillUniformFloat(BNNSRandomGenerator?, UnsafeMutablePointer&lt;BNNSNDArrayDescriptor>, Float, Float) -> Int32

Fills the specified tensor with random floating-point values from the continuous uniform distribution within a range.

func BNNSRandomFillNormalFloat(BNNSRandomGenerator?, UnsafeMutablePointer&lt;BNNSNDArrayDescriptor>, Float, Float) -> Int32

Fills the specified tensor with random floating-point values mapped to a normal distribution.

func BNNSRandomFillCategoricalFloat(BNNSRandomGenerator?, UnsafePointer&lt;BNNSNDArrayDescriptor>, UnsafePointer&lt;BNNSNDArrayDescriptor>, Bool) -> Int32

Fills the specified tensor with random values from the categorical distributions with the given event probabilities.

func BNNSRandomGeneratorStateSize(BNNSRandomGenerator?) -> Int

Returns the state size, in bytes, of a random number generator.

func BNNSRandomGeneratorGetState(BNNSRandomGenerator?, Int, UnsafeMutableRawPointer) -> Int32

Returns the state of a random number generator.

func BNNSDestroyRandomGenerator(BNNSRandomGenerator?)

Destroys a random number generator.

