

- Accelerate
- BNNSNDArrayDescriptor
-  allocate(randomUniformUsing:range:shape:batchSize:) 

Type Method

# allocate(randomUniformUsing:range:shape:batchSize:)

Returns a new array descriptor that’s initialized with random integer values from the continuous uniform distribution.

iOS 15.0+iPadOS 15.0+Mac CatalystmacOS 12.0+tvOS 15.0+visionOSwatchOS 8.0+

``` source
static func allocate(
    randomUniformUsing: BNNS.RandomGenerator,
    range: ClosedRange,
    shape: BNNS.Shape,
    batchSize: Int = 1
) -> BNNSNDArrayDescriptor? where Scalar : BNNSScalar, Scalar : BinaryFloatingPoint
```

## Parameters 

`randomUniformUsing`  

The random number generator that provides random values.

`range`  

The range of random values.

`shape`  

The shape of the n-dimensional array descriptor.

`batchSize`  

The number of batches of data.

## Discussion

Use this function to create a new array descriptor that’s initialized with random values BNNS.RandomGenerator generates.

If you use the same generator on multiple threads, note that this function serializes the generator through an internal lock. To eliminate this contention, use different generators for each thread.

The following code creates a 16-element 1D tensor that contains random 16-bit integer values between `-10` and `10`:

```
guard
    let randomGenerator = BNNS.RandomGenerator(
        method: .aesCtr,
        seed: 1234),
    let descriptor = BNNSNDArrayDescriptor.allocate(
        randomUniformUsing: randomGenerator,
        range: Int16(-10)...Int16(10),
        shape: [16]) else {
        return
    }

// Prints 16 random values.
print(descriptor.makeArray(of: Int16.self)!)

descriptor.deallocate()
```

## See Also

### Allocating and Deallocating Memory

static func allocate&lt;C>(initializingFrom: C, shape: BNNS.Shape, batchSize: Int) -> BNNSNDArrayDescriptor

Returns a new n-dimensional array descriptor that’s initialized with a copy of the elements in the specified collection.

static func allocate&lt;Scalar>(randomUniformUsing: BNNS.RandomGenerator, range: ClosedRange&lt;Scalar>, shape: BNNS.Shape, batchSize: Int) -> BNNSNDArrayDescriptor?

Returns a new array descriptor that’s initialized with random floating-point values from the continuous uniform distribution.

static func allocate&lt;Scalar>(randomIn: ClosedRange&lt;Scalar>, shape: BNNS.Shape, batchSize: Int) -> BNNSNDArrayDescriptor

Returns a new n-dimensional array descriptor that’s initialized with random values within the specified range.

static func allocate&lt;Scalar>(randomIn: ClosedRange&lt;Scalar>, shape: BNNS.Shape, batchSize: Int) -> BNNSNDArrayDescriptor

Returns a new n-dimensional array descriptor that’s initialized with random values within the specified range.

static func allocate&lt;Scalar, Generator>(randomIn: ClosedRange&lt;Scalar>, using: inout Generator, shape: BNNS.Shape, batchSize: Int) -> BNNSNDArrayDescriptor

Returns a new array descriptor that’s initialized with random values within the specified range, using the given generator as a source for randomness.

static func allocate&lt;Scalar, Generator>(randomIn: ClosedRange&lt;Scalar>, using: inout Generator, shape: BNNS.Shape, batchSize: Int) -> BNNSNDArrayDescriptor

Returns a new array descriptor that’s initialized with random values within the specified range, using the given generator as a source for randomness.

static func allocate&lt;T>(repeating: T, shape: BNNS.Shape, batchSize: Int) -> BNNSNDArrayDescriptor

Returns a new n-dimensional array descriptor that’s initialized with a single, repeated scalar value.

static func allocateUninitialized(scalarType: any BNNSScalar.Type, shape: BNNS.Shape, batchSize: Int) -> BNNSNDArrayDescriptor

Returns a new n-dimensional array descriptor that’s allocated with uninitialized memory.

func deallocate()

Deallocates the memory block previously allocated to this n-dimensional array descriptor.

