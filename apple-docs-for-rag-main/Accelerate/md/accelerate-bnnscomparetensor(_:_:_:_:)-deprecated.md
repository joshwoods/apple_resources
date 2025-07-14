

- Accelerate
-  BNNSCompareTensor(\_:\_:\_:\_:) Deprecated

Function

# BNNSCompareTensor(\_:\_:\_:\_:)

Returns a tensor of Boolean type by comparing or performing a logical operation between two inputs.

iOS 14.0–18.0DeprecatediPadOS 14.0–18.0DeprecatedMac Catalyst 14.0–18.0DeprecatedmacOS 11.0–15.0DeprecatedtvOS 14.0–18.0DeprecatedvisionOS 1.0–2.0DeprecatedwatchOS 7.0–11.0Deprecated

``` source
func BNNSCompareTensor(
    _ in0: UnsafePointer,
    _ in1: UnsafePointer,
    _ op: BNNSRelationalOperator,
    _ out: UnsafeMutablePointer
) -> Int32
```

Deprecated

Use BNNSGraph\* APIs

## Parameters 

`in0`  

The descriptor of the first input.

`in1`  

The descriptor of the second input.

`op`  

The operator for comparison.

`out`  

The descriptor of the output.

## Discussion

Use relational operators, for example BNNSRelationalOperatorGreater and BNNSRelationalOperatorLess, to compare floating-point elements. The following code compares the elements of two arrays of single-precision values for equality:

```
let a: [Float] = [1, 2, 3, 4]
let b: [Float] = [5, 4, 3, 2]

let size = (a.count, 0, 0, 0, 0, 0, 0, 0)
let stride = (0, 0, 0, 0, 0, 0, 0, 0)

var destination = [Bool](repeating: false,
                         count: size.0)

a.withUnsafeBufferPointer { aPtr in
    b.withUnsafeBufferPointer { bPtr in
        destination.withUnsafeMutableBufferPointer { destinationPtr in
            var aDescription = BNNSNDArrayDescriptor(flags: BNNSNDArrayFlags(0),
                                                     layout: BNNSDataLayoutVector,
                                                     size: size,
                                                     stride: stride,
                                                     data: UnsafeMutableRawPointer(mutating: aPtr.baseAddress!),
                                                     data_type: .float,
                                                     table_data: nil,
                                                     table_data_type: .float,
                                                     data_scale: 1,
                                                     data_bias: 0)

            var bDescription = BNNSNDArrayDescriptor(flags: BNNSNDArrayFlags(0),
                                                     layout: BNNSDataLayoutVector,
                                                     size: size,
                                                     stride: stride,
                                                     data: UnsafeMutableRawPointer(mutating: bPtr.baseAddress!),
                                                     data_type: .float,
                                                     table_data: nil,
                                                     table_data_type: .float,
                                                     data_scale: 1,
                                                     data_bias: 0)

            var destinationDescription = BNNSNDArrayDescriptor(flags: BNNSNDArrayFlags(0),
                                                               layout: BNNSDataLayoutVector,
                                                               size: size,
                                                               stride: stride,
                                                               data: destinationPtr.baseAddress!,
                                                               data_type: BNNSDataTypeBoolean,
                                                               table_data: nil,
                                                               table_data_type: BNNSDataTypeBoolean,
                                                               data_scale: 1,
                                                               data_bias: 0)

            BNNSCompareTensor(&aDescription,
                              &bDescription,
                              BNNSRelationalOperatorEqual,
                              &destinationDescription)
        }
    }
}
```

On return, `destination` contains the values `[false, false, true, false]`.

Use logical operators, for example BNNSRelationalOperatorLogicalAND and BNNSRelationalOperatorLogicalOR, to compare Boolean elements. The following code performs a logical AND operation on the elements of two arrays of Boolean values:

```

let a: [Bool] = [ true, false, false, true]
let b: [Bool] = [false, false,  true, true]

let size = (a.count, 0, 0, 0, 0, 0, 0, 0)
let stride = (0, 0, 0, 0, 0, 0, 0, 0)

var destination = [Bool](repeating: false,
                         count: size.0)

a.withUnsafeBufferPointer { aPtr in
    b.withUnsafeBufferPointer { bPtr in
        destination.withUnsafeMutableBufferPointer { destinationPtr in
            var aDescription = BNNSNDArrayDescriptor(flags: BNNSNDArrayFlags(0),
                                                     layout: BNNSDataLayoutVector,
                                                     size: size,
                                                     stride: stride,
                                                     data: UnsafeMutableRawPointer(mutating: aPtr.baseAddress!),
                                                     data_type: BNNSDataTypeBoolean,
                                                     table_data: nil,
                                                     table_data_type: BNNSDataTypeBoolean,
                                                     data_scale: 1,
                                                     data_bias: 0)

            var bDescription = BNNSNDArrayDescriptor(flags: BNNSNDArrayFlags(0),
                                                     layout: BNNSDataLayoutVector,
                                                     size: size,
                                                     stride: stride,
                                                     data: UnsafeMutableRawPointer(mutating: bPtr.baseAddress!),
                                                     data_type: BNNSDataTypeBoolean,
                                                     table_data: nil,
                                                     table_data_type: BNNSDataTypeBoolean,
                                                     data_scale: 1,
                                                     data_bias: 0)

            var destinationDescription = BNNSNDArrayDescriptor(flags: BNNSNDArrayFlags(0),
                                                               layout: BNNSDataLayoutVector,
                                                               size: size,
                                                               stride: stride,
                                                               data: destinationPtr.baseAddress!,
                                                               data_type: BNNSDataTypeBoolean,
                                                               table_data: nil,
                                                               table_data_type: BNNSDataTypeBoolean,
                                                               data_scale: 1,
                                                               data_bias: 0)

            BNNSCompareTensor(&aDescription,
                              &bDescription,
                              BNNSRelationalOperatorLogicalAND,
                              &destinationDescription)

        }
    }
}
```

On return, `destination` contains the values `[false, false, false, true]`.

## See Also

### Tensor comparison layers

static func compare(BNNSNDArrayDescriptor, BNNSNDArrayDescriptor, using: BNNS.RelationalOperator, output: BNNSNDArrayDescriptor) throws

Performs an elementwise comparison of two array descriptors using the specified relational operator.

Deprecated

struct BNNSRelationalOperator

Constants that describe relational operations.

