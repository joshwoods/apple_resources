

- ML Compute
- MLCTensor
-  bindOptimizerData(\_:deviceData:) Deprecated

Instance Method

# bindOptimizerData(\_:deviceData:)

Associates the optimizer and device data buffers you specify to the tensor.

iOS 14.0–17.4DeprecatediPadOS 14.0–17.4DeprecatedMac Catalyst 14.0–17.4DeprecatedmacOS 11.0–14.3DeprecatedtvOS 14.0–17.4Deprecated

``` source
func bindOptimizerData(
    _ data: [MLCTensorData],
    deviceData: [MLCTensorOptimizerDeviceData]?
) -> Bool
```

## Parameters 

`data`  

An array that contains the optimizer data to associate with the tensor.

`deviceData`  

An array that contains the optimizer device data to associate with the tensor.

## Return Value

`true` if the framework successfully associated the data and device data with the tensor; otherwise, `false`.

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

func bindAndWriteData(MLCTensorData, to: MLCDevice) -> Bool

Associates the given data to the tensor, and if the device is a GPU, also copies the data to the device memory.

Deprecated

