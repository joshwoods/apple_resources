

- Accelerate
-  BNNSRandomFillUniformFloat(\_:\_:\_:\_:) 

Function

# BNNSRandomFillUniformFloat(\_:\_:\_:\_:)

Fills the specified tensor with random floating-point values from the continuous uniform distribution within a range.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
func BNNSRandomFillUniformFloat(
    _ generator: BNNSRandomGenerator?,
    _ desc: UnsafeMutablePointer,
    _ a: Float,
    _ b: Float
) -> Int32
```

## Parameters 

`generator`  

The random number generator.

`desc`  

The descriptor of the destination.

`a`  

The lower bound of distribution.

`b`  

The upper bound of distribution.

## Discussion

Use this function to fill an array descriptor with uniformly distributed random values.

If you use the same generator on multiple threads, note that this function serializes the generator through an internal lock. To eliminate this contention, use different generators for each thread.

If the descriptor’s data_type isn’t 32-bit floating point, the values that you specify for the bounds must be exactly representable in the descriptor’s data type.

The following code populates a descriptor with random floating-point values:

```
let data = UnsafeMutableBufferPointer.allocate(capacity: 8)
var descriptor = BNNSNDArrayDescriptor(flags: BNNSNDArrayFlags(0),
                                       layout: BNNSDataLayoutVector,
                                       size: (10, 0, 0, 0, 0, 0, 0, 0),
                                       stride: (0, 0, 0, 0, 0, 0, 0, 0),
                                       data: data.baseAddress!,
                                       data_type: BNNSDataType.float,
                                       table_data: nil,
                                       table_data_type: BNNSDataType.float,
                                       data_scale: 1, data_bias: 0)

guard let randomNumberGenerator = BNNSCreateRandomGenerator(BNNSRandomGeneratorMethodAES_CTR,
                                                            nil) else {
    return
}

BNNSRandomFillUniformFloat(randomNumberGenerator,
                           &descriptor,
                           -10,
                           10)

print(Array(data))

data.deallocate()
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

func BNNSRandomFillNormalFloat(BNNSRandomGenerator?, UnsafeMutablePointer&lt;BNNSNDArrayDescriptor>, Float, Float) -> Int32

Fills the specified tensor with random floating-point values mapped to a normal distribution.

func BNNSRandomFillCategoricalFloat(BNNSRandomGenerator?, UnsafePointer&lt;BNNSNDArrayDescriptor>, UnsafePointer&lt;BNNSNDArrayDescriptor>, Bool) -> Int32

Fills the specified tensor with random values from the categorical distributions with the given event probabilities.

func BNNSRandomGeneratorStateSize(BNNSRandomGenerator?) -> Int

Returns the state size, in bytes, of a random number generator.

func BNNSRandomGeneratorGetState(BNNSRandomGenerator?, Int, UnsafeMutableRawPointer) -> Int32

Returns the state of a random number generator.

func BNNSRandomGeneratorSetState(BNNSRandomGenerator?, Int, UnsafeMutableRawPointer) -> Int32

Sets the state of a random number generator.

func BNNSDestroyRandomGenerator(BNNSRandomGenerator?)

Destroys a random number generator.

