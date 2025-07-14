

- Accelerate
-  BNNSRandomFillCategoricalFloat(\_:\_:\_:\_:) 

Function

# BNNSRandomFillCategoricalFloat(\_:\_:\_:\_:)

Fills the specified tensor with random values from the categorical distributions with the given event probabilities.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
func BNNSRandomFillCategoricalFloat(
    _ generator: BNNSRandomGenerator?,
    _ desc: UnsafePointer,
    _ probabilities: UnsafePointer,
    _ log_probabilities: Bool
) -> Int32
```

## Parameters 

`generator`  

The random number generator.

`desc`  

The descriptor of the destination.

`probabilities`  

The descriptor of the probabilities.

`log_probabilities`  

A Boolean value that specifies whether the probabilities descriptor contains event log probabilities.

## Discussion

Use this function to fill an array descriptor with random values from a categorical distribution with specified event probabilities or event log probabilities.

If you use the same generator on multiple threads, note that this function serializes the generator through an internal lock. To eliminate this contention, use different generators for each thread.

The size and shape of the output descriptor, `desc`, is dependent on the probabilities descriptor. The output descriptor must have the same rank as the probabilities descriptor. The first `rank-1` dimensions of the output descriptor must be the same size as the first `rank-1` dimensions of the probabilities descriptor.

The function treats the first `rank-1` dimensions as batch sizes. On return, the output descriptor contains random integers in the range `[0,1,…,K-1]`, where `K` is the dimension and the number of events.

Supply the probabilities data as nonnegative and finite values. The function normalizes the probabilities values along the innermost dimension so that the probability values (or their exponentials) sum to one along the innermost dimension.

For example, the following code fills an array descriptor with 1024 random integer values between `0` and `14`. The `probabilities` descriptor specifies the likelihood of the random generator selecting any particular value. For example, BNNSRandomFillCategoricalFloat(_:_:_:_:) never selects `0` or `1`, and is twice as likely to select `3` (with a probability of `10`) than `2` (with a probability of `5`).

```
 var desc = BNNSNDArrayDescriptor.allocateUninitialized(scalarType: Float.self,
                                                        shape: .vector(1024))

 let probs: [Float] = normalize([0, 0, 5, 10, 8, 6, 4, 2, 0, 0, 5, 10, 5, 0, 0])

 var probabilities = BNNSNDArrayDescriptor.allocate(initializingFrom: probs,
                                                    shape: .vector(probs.count))

 let rng = BNNSCreateRandomGenerator(BNNSRandomGeneratorMethodAES_CTR,
                                     nil);

 let error = BNNSRandomFillCategoricalFloat(rng, &desc, &probabilities, false)

 defer {
     BNNSDestroyRandomGenerator(rng)
 }
```

The following graph shows the normalized event probabilities as a line chart and a histogram of the normalized random values as a bar chart:

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

func BNNSRandomGeneratorStateSize(BNNSRandomGenerator?) -> Int

Returns the state size, in bytes, of a random number generator.

func BNNSRandomGeneratorGetState(BNNSRandomGenerator?, Int, UnsafeMutableRawPointer) -> Int32

Returns the state of a random number generator.

func BNNSRandomGeneratorSetState(BNNSRandomGenerator?, Int, UnsafeMutableRawPointer) -> Int32

Sets the state of a random number generator.

func BNNSDestroyRandomGenerator(BNNSRandomGenerator?)

Destroys a random number generator.

