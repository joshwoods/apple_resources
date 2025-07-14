

- ML Compute
- MLCTensor
-  bindAndWriteData(\_:to:) Deprecated

Instance Method

# bindAndWriteData(\_:to:)

Associates the given data to the tensor, and if the device is a GPU, also copies the data to the device memory.

iOS 14.0–17.4DeprecatediPadOS 14.0–17.4DeprecatedMac Catalyst 14.0–17.4DeprecatedmacOS 11.0–14.3DeprecatedtvOS 14.0–17.4Deprecated

``` source
func bindAndWriteData(
    _ data: MLCTensorData,
    to device: MLCDevice
) -> Bool
```

## Parameters 

`data`  

The data you want to associate with the tensor.

`device`  

The compute device.

## Return Value

`true` if the framework successfully associated the data with the tensor and copied it to the device; otherwise, `false`.

## Discussion

The caller must guarantee the lifetime of the underlying memory of `data` for the lifetime of the tensor.

Only use this method to update device memory for tensors that are typically layer parameters, such as weights and bias for convolution layers, or beta and gamma for normalization layers. A typical use case might be implementing your own optimizer and needing to update the device memory data for these tensors.

For input tensors, use bindAndWriteData(_:forInputs:to:batchSize:synchronous:).

## See Also

### Managing Tensor Data

func synchronizeData() -> Bool

Synchronizes the data in host memory.

Deprecated

func synchronizeOptimizerData() -> Bool

Synchronizes the optimizer data in host memory.

Deprecated

func copyDataFromDeviceMemory(toBytes: UnsafeMutableRawPointer, length: Int, synchronizeWithDevice: Bool) -> Bool

Copies tensor data from device memory to user-specified memory.

Deprecated

func bindOptimizerData([MLCTensorData], deviceData: [MLCTensorOptimizerDeviceData]?) -> Bool

Associates the optimizer and device data buffers you specify to the tensor.

Deprecated

