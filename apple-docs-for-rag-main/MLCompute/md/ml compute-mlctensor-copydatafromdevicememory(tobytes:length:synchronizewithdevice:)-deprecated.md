

- ML Compute
- MLCTensor
-  copyDataFromDeviceMemory(toBytes:length:synchronizeWithDevice:) Deprecated

Instance Method

# copyDataFromDeviceMemory(toBytes:length:synchronizeWithDevice:)

Copies tensor data from device memory to user-specified memory.

iOS 14.0–17.4DeprecatediPadOS 14.0–17.4DeprecatedMac Catalyst 14.0–17.4DeprecatedmacOS 11.0–14.3DeprecatedtvOS 14.0–17.4Deprecated

``` source
func copyDataFromDeviceMemory(
    toBytes bytes: UnsafeMutableRawPointer,
    length: Int,
    synchronizeWithDevice: Bool
) -> Bool
```

## Parameters 

`bytes`  

The data to copy.

`length`  

The number of bytes you specify for the framework to copy.

`synchronizeWithDevice`  

A Boolean that indicates whether you choose to synchronize device memory if the device is a GPU.

## Return Value

`true` if successful; otherwise, `false` if the framework failed to copy or synchronize.

## Discussion

When the device is a GPU, you may need to synchronize the device memory, that is, set `synchronizeWithDevice` to `true`. The framework ignores `synchronizeWithDevice` when the device is the CPU.

Important

Only call this method once the graph, with which you used this tensor, finishes execution. Otherwise the results in device memory may not be up to date. When the device is a GPU, you must set `synchronizeWithDevice` to `false` when you call this method in a completion handler. If you specified a tensor for the outputs of a graph using `addOutputs`, set `synchronizeWithDevice` to `false`.

## See Also

### Managing Tensor Data

func synchronizeData() -> Bool

Synchronizes the data in host memory.

Deprecated

func synchronizeOptimizerData() -> Bool

Synchronizes the optimizer data in host memory.

Deprecated

func bindAndWriteData(MLCTensorData, to: MLCDevice) -> Bool

Associates the given data to the tensor, and if the device is a GPU, also copies the data to the device memory.

Deprecated

func bindOptimizerData([MLCTensorData], deviceData: [MLCTensorOptimizerDeviceData]?) -> Bool

Associates the optimizer and device data buffers you specify to the tensor.

Deprecated

