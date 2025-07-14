

- Accelerate
-  BNNSRandomGeneratorMethod 

Structure

# BNNSRandomGeneratorMethod

Constants that describe random number generation methods.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
struct BNNSRandomGeneratorMethod
```

## Topics

### Random Number Generation Methods

init(UInt32)

Creates a new instance with the specified raw value.

init(rawValue: UInt32)

Creates a new instance with the specified raw value.

var rawValue: UInt32

The corresponding value of the raw type.

var BNNSRandomGeneratorMethodAES_CTR: BNNSRandomGeneratorMethod

A constant that specifes an implementation that’s based on the Advanced Encryption Standard (AES) hash of a counter.

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Random number generation

class RandomGenerator

A random number generator.

func BNNSCreateRandomGenerator(BNNSRandomGeneratorMethod, UnsafePointer&lt;BNNSFilterParameters>?) -> BNNSRandomGenerator?

Returns a new random number generator using an internally generated random seed.

func BNNSCreateRandomGeneratorWithSeed(BNNSRandomGeneratorMethod, UInt64, UnsafePointer&lt;BNNSFilterParameters>?) -> BNNSRandomGenerator?

Returns a new random number generator using the specified seed.

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

func BNNSRandomGeneratorSetState(BNNSRandomGenerator?, Int, UnsafeMutableRawPointer) -> Int32

Sets the state of a random number generator.

func BNNSDestroyRandomGenerator(BNNSRandomGenerator?)

Destroys a random number generator.

