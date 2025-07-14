

- ML Compute
- MLCTensor
-  synchronizeData() Deprecated

Instance Method

# synchronizeData()

Synchronizes the data in host memory.

iOS 14.0–17.4DeprecatediPadOS 14.0–17.4DeprecatedMac Catalyst 14.0–17.4DeprecatedmacOS 11.0–14.3DeprecatedtvOS 14.0–17.4Deprecated

``` source
func synchronizeData() -> Bool
```

## Return Value

`true` if synchronization is successful; otherwise, `false`.

## Discussion

This method synchronizes the tensor’s data in host memory with the latest contents in device memory.

Only call this method once the graph, with which you used this tensor, finishes execution; otherwise the results in device memory may not be up to date.

Important

Don’t call this method from a completion callback when the device is a GPU.

## See Also

### Managing Tensor Data

func synchronizeOptimizerData() -> Bool

Synchronizes the optimizer data in host memory.

Deprecated

func copyDataFromDeviceMemory(toBytes: UnsafeMutableRawPointer, length: Int, synchronizeWithDevice: Bool) -> Bool

Copies tensor data from device memory to user-specified memory.

Deprecated

func bindAndWriteData(MLCTensorData, to: MLCDevice) -> Bool

Associates the given data to the tensor, and if the device is a GPU, also copies the data to the device memory.

Deprecated

func bindOptimizerData([MLCTensorData], deviceData: [MLCTensorOptimizerDeviceData]?) -> Bool

Associates the optimizer and device data buffers you specify to the tensor.

Deprecated

