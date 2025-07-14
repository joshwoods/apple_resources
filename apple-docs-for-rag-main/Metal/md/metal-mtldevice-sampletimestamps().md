

- Metal
- MTLDevice
-  sampleTimestamps() 

Instance Method

# sampleTimestamps()

Captures and returns a CPU timestamp and a GPU timestamp from the same moment in time.

iOS 14.0+iPadOS 14.0+Mac CatalystmacOS 11.0+tvOS 14.0+visionOS

``` source
func sampleTimestamps() -> (cpu: MTLTimestamp, gpu: MTLTimestamp)
```

## Return Value

A tuple that contains the CPU and GPU timestamps.

`cpu`  
A timestamp from the CPU.

`gpu`  
A timestamp from the GPU the device instance represents.

## Mentioned in 

Converting GPU Timestamps into CPU Time

Converting a GPU’s Counter Data into a Readable Format

## Discussion

For an example of how and when to use corresponding timestamps from the CPU and GPU, see Converting GPU Timestamps into CPU Time.

