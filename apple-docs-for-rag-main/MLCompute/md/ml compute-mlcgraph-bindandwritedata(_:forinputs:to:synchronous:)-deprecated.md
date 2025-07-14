

- ML Compute
- MLCGraph
-  bindAndWriteData(\_:forInputs:to:synchronous:) Deprecated

Instance Method

# bindAndWriteData(\_:forInputs:to:synchronous:)

Associates the given data with the input tensors, and if the device is a GPU, also copies the data to the device memory.

iOS 14.0–17.4DeprecatediPadOS 14.0–17.4DeprecatedMac Catalyst 14.0–17.4DeprecatedmacOS 11.0–14.3DeprecatedtvOS 14.0–17.4Deprecated

``` source
func bindAndWriteData(
    _ inputsData: [String : MLCTensorData],
    forInputs inputTensors: [String : MLCTensor],
    to device: MLCDevice,
    synchronous: Bool
) -> Bool
```

## Parameters 

`inputsData`  

An array that contains the input data to write to device memory.

`inputTensors`  

The list of tensors to perform writes on.

`device`  

The compute device.

`synchronous`  

A Boolean value that indicates whether to execute the copy to the device synchronously.

## Return Value

`true` if the data is successfully associated with input tensors, otherwise `false`.

## Discussion

Use this method if you execute the forward, gradient, and optimizer updates independently. Write the inputs to device memory before the layer executes the forward pass. Similarly, write the inputs—typically the initial gradient tensor—to device memory before the layer executes the gradient pass.

Use asynchronous execution for better performance, except when testing or debugging.

Important

You must guarantee the lifetime of the underlying memory of each value of `inputsData` for the entirety of each corresponding input tensor’s lifetime.

## See Also

### Associating Data with Input Tensors

func bindAndWriteData([String : MLCTensorData], forInputs: [String : MLCTensor], to: MLCDevice, batchSize: Int, synchronous: Bool) -> Bool

Associates the given data with the input tensors, and if the device is a GPU, also copies the data to the device memory.

Deprecated

