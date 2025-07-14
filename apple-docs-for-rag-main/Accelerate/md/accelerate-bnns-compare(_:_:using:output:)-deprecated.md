

- Accelerate
- BNNS
-  compare(\_:\_:using:output:) Deprecated

Type Method

# compare(\_:\_:using:output:)

Performs an elementwise comparison of two array descriptors using the specified relational operator.

iOS 14.0+iPadOS 14.0+Mac CatalystmacOS 11.0+tvOS 14.0+visionOSwatchOS 7.0+

``` source
static func compare(
    _ inputA: BNNSNDArrayDescriptor,
    _ inputB: BNNSNDArrayDescriptor,
    using relationalOperator: BNNS.RelationalOperator,
    output: BNNSNDArrayDescriptor
) throws
```

Deprecated

Use the BNNSGraph API instead.

## Parameters 

`inputA`  

The descriptor of the first input.

`inputB`  

The descriptor of the second input.

`relationalOperator`  

The operator for comparison.

`output`  

The descriptor of the output.

## Topics

### Specifying a Relational Operator

struct RelationalOperator

Constants that describe relational operations.

## See Also

### Tensor comparison layers

struct BNNSRelationalOperator

Constants that describe relational operations.

func BNNSCompareTensor(UnsafePointer&lt;BNNSNDArrayDescriptor>, UnsafePointer&lt;BNNSNDArrayDescriptor>, BNNSRelationalOperator, UnsafeMutablePointer&lt;BNNSNDArrayDescriptor>) -> Int32

Returns a tensor of Boolean type by comparing or performing a logical operation between two inputs.

Deprecated

