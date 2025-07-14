

- Accelerate
-  BNNSDirectApplyInTopK(\_:\_:\_:\_:\_:\_:\_:\_:\_:\_:) 

Function

# BNNSDirectApplyInTopK(\_:\_:\_:\_:\_:\_:\_:\_:\_:\_:)

Applies an in-top-k filter directly to an input.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
func BNNSDirectApplyInTopK(
    _ K: Int,
    _ axis: Int,
    _ batch_size: Int,
    _ input: UnsafePointer,
    _ input_batch_stride: Int,
    _ test_indices: UnsafePointer,
    _ test_indices_batch_stride: Int,
    _ output: UnsafeMutablePointer,
    _ output_batch_stride: Int,
    _ filter_params: UnsafePointer?
) -> Int32
```

## Parameters 

`K`  

The number of entries the operation finds.

`axis`  

The axis along which the operation finds top-k entries.

`batch_size`  

Number of input-output pairs to process.

`input`  

The descriptor of the input.

`input_batch_stride`  

Increment, in values, between inputs.

`test_indices`  

The descriptor of the test indices.

`test_indices_batch_stride`  

Increment, in values, between test indices tensors.

`output`  

The descriptor of the output.

`output_batch_stride`  

Increment, in values, between outputs.

`filter_params`  

The filter runtime parameters.

## Discussion

Use BNNSDirectApplyInTopK(_:_:_:_:_:_:_:_:_:_:) to test whether elements in a tensor are in the top k entries. Note the the number of dimensions for the test indices and output tensors are one less than the input tensor.

Important

The input data type must be `float`, the test indices data type must be `int32`, and the output data type must be `BNNSDataTypeBoolean`.

For example, given the following 4 x 4 row-major matrix and vector of test indices:

```
let source: [Float] = [1, 2, 3, 9,
                       1, 6, 7, 1,
                       9, 0, 1, 3,
                       4, 5, 8, 1]

let testIndices: [Int32] = [3, 2, 1, 0]
```

The following code checks the values in source are in the top k entries for each successive row:

```
var output = [Bool](repeating: false,
                    count: testIndices.count)

let n = 4
let k = 2

source.withUnsafeBufferPointer { srcPtr in
    testIndices.withUnsafeBufferPointer { testIndicesPtr in
        output.withUnsafeMutableBytes { outputPtr in

            var inputDescriptor = BNNSNDArrayDescriptor(flags: BNNSNDArrayFlags(0),
                                                        layout: BNNSDataLayoutRowMajorMatrix,
                                                        size: (n, n, 0, 0, 0, 0, 0, 0),
                                                        stride: (0, 0, 0, 0, 0, 0, 0, 0),
                                                        data: UnsafeMutableRawPointer(mutating: srcPtr.baseAddress),
                                                        data_type: .float,
                                                        table_data: nil,
                                                        table_data_type: .float,
                                                        data_scale: 1,
                                                        data_bias: 0)

            var testIndicesDescriptor = BNNSNDArrayDescriptor(flags: BNNSNDArrayFlags(0),
                                                              layout: BNNSDataLayoutVector,
                                                              size: (n, 0, 0, 0, 0, 0, 0, 0),
                                                              stride: (0, 0, 0, 0, 0, 0, 0, 0),
                                                              data: UnsafeMutableRawPointer(mutating: testIndicesPtr.baseAddress),
                                                              data_type: .int32,
                                                              table_data: nil,
                                                              table_data_type: .int32,
                                                              data_scale: 1,
                                                              data_bias: 0)

            var outputDescriptor = BNNSNDArrayDescriptor(flags: BNNSNDArrayFlags(0),
                                                         layout: BNNSDataLayoutVector,
                                                         size: (n, 0, 0, 0, 0, 0, 0, 0),
                                                         stride: (0, 0, 0, 0, 0, 0, 0, 0),
                                                         data: outputPtr.baseAddress,
                                                         data_type: BNNSDataTypeBoolean,
                                                         table_data: nil,
                                                         table_data_type: .float,
                                                         data_scale: 1,
                                                         data_bias: 0)

            BNNSDirectApplyInTopK(k,
                                  1,
                                  1,
                                  &inputDescriptor, n * n,
                                  &testIndicesDescriptor, n,
                                  &outputDescriptor, n,
                                  nil)
        }
    }
}
```

On return, the output contains `[true, true, false, false]`. The operation calculates these values as:

- `true`: element `3` of the first row of `source` is `9.0` which is in the top 2 (`3.0, 9.0`).

- `true`: element `2` of the second row of `source` is `7.0` which is in the top 2 (`6.0, 7.0`).

- `false`: element `1` of the third row of `source` is `0.0` which isn’t in the top 2 (`3.0, 9.0`).

- `false`: element `0` of the fourth row of `source` is `4.0` which isn’t in the top 2 (`5.0, 8.0`).

## See Also

### Top-k layers

func BNNSDirectApplyTopK(Int, Int, Int, UnsafePointer&lt;BNNSNDArrayDescriptor>, Int, UnsafeMutablePointer&lt;BNNSNDArrayDescriptor>, Int, UnsafeMutablePointer&lt;BNNSNDArrayDescriptor>?, Int, UnsafePointer&lt;BNNSFilterParameters>?) -> Int32

Applies a top-k filter directly to an input.

