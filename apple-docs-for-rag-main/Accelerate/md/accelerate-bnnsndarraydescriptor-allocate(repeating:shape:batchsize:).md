

- Accelerate
- BNNSNDArrayDescriptor
-  allocate(repeating:shape:batchSize:) 

Type Method

# allocate(repeating:shape:batchSize:)

Returns a new n-dimensional array descriptor that’s initialized with a single, repeated scalar value.

iOS 14.0+iPadOS 14.0+Mac CatalystmacOS 11.0+tvOS 14.0+visionOSwatchOS 7.0+

``` source
static func allocate(
    repeating repeatedValue: T,
    shape: BNNS.Shape,
    batchSize: Int = 1
) -> BNNSNDArrayDescriptor where T : BNNSScalar
```

## Parameters 

`repeatedValue`  

The element to repeat.

`shape`  

The shape of n-dimensional array descriptor.

`batchSize`  

The number of batches of data.

## See Also

### Allocating and Deallocating Memory

static func allocate&lt;C>(initializingFrom: C, shape: BNNS.Shape, batchSize: Int) -> BNNSNDArrayDescriptor

Returns a new n-dimensional array descriptor that’s initialized with a copy of the elements in the specified collection.

static func allocate&lt;Scalar>(randomUniformUsing: BNNS.RandomGenerator, range: ClosedRange&lt;Scalar>, shape: BNNS.Shape, batchSize: Int) -> BNNSNDArrayDescriptor?

Returns a new array descriptor that’s initialized with random integer values from the continuous uniform distribution.

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

static func allocateUninitialized(scalarType: any BNNSScalar.Type, shape: BNNS.Shape, batchSize: Int) -> BNNSNDArrayDescriptor

Returns a new n-dimensional array descriptor that’s allocated with uninitialized memory.

func deallocate()

Deallocates the memory block previously allocated to this n-dimensional array descriptor.

