

- Metal
- GPU Counters and Counter Sample Buffers
-  Converting a GPU’s Counter Data into a Readable Format 

Article

# Converting a GPU’s Counter Data into a Readable Format

Inspect and use the data within a GPU’s counter sample buffer by resolving it into a standard format.

## Overview

To use the data a GPU driver stores in an MTLCounterSampleBuffer instance (see Sampling GPU Data into Counter Sample Buffers), your app must *resolve* it. Resolving the data converts the counter data from the GPU’s internal data structure into a common format that Metal defines.

You can resolve the data in a counter sample buffer by creating a blit pass that converts the data as it copies it to an MTLBuffer. If the CPU can access a counter sample buffer, you can also resolve the data after the GPU finishes running a command buffer. See Creating a Counter Sample Buffer to Store a GPU’s Counter Data During a Pass for information about making a CPU-accessible counter sample buffer.

### Resolve the Counter Sample Buffer with the CPU

For an MTLCounterSampleBuffer instance that you create with shared memory (see storageMode and MTLStorageMode.shared), you can resolve the data by calling its resolveCounterRange(_:) method.

- Swift
- Objective-C

```
/// Converts the contents of the counter sample buffer into an array of result timestamps.
func resolveSampleBuffer() {
    /// Represents the size of the counter sample buffer.
    let range = 0..

```
/// Converts the contents of the counter sample buffer into an array of result timestamps.- (void) resolveSampleBuffer
{
    /// Represents the size of the counter sample buffer.
    NSRange range = NSMakeRange(0, self.sampleCount);

    // Convert the contents of the counter sample buffer into the standard data format.
    NSData* data = [self.counterSampleBuffer resolveCounterRange:range];
    if (nil == data) {
        return;
    }
    ...
}
```

You can resolve a sample counter buffer with the CPU at any time after the GPU finishes running the pass that retrieves the counter’s data. To access the data as soon as possible (with the CPU), add a completion handler to the pass’s command buffer by calling its addCompletedHandler(_:) method.

- Swift
- Objective-C

```
commandBuffer.addCompletedHandler { commandBuffer in
    let timestamps = func resolveSampleBuffer() {
    ...
}
```

```
[commandBuffer addCompletedHandler:^(id _Nonnull commandBuffer) {
    [self resolveSampleBuffer];
    ...
}];
```

### Resolve the Counter Sample Buffer with a Blit Pass on the GPU

You can also resolve an MTLCounterSampleBuffer instance’s data into an MTLBuffer by running a blit pass on the GPU. For some GPUs, this technique is the only way to resolve a counter sample buffer that uses private storage (see storageMode and MTLStorageMode.private).

To resolve a sample counter buffer in a blit pass, create an MTLBlitCommandEncoder instance and call its resolveCounters(_:range:destinationBuffer:destinationOffset:) method.

- Swift
- Objective-C

```
func resolveSampleBuffer(_ sampleBuffer: MTLCounterSampleBuffer,
                         with blitEncoder: MTLBlitCommandEncoder,
                         toBufferWith resourceOptions: MTLResourceOptions) -> MTLBuffer? {

    let counterBufferLength = MemoryLayout.size * sampleCount
    let counterDataBuffer = sampleBuffer.device.makeBuffer(length: counterBufferLength,
                                                           options: resourceOptions)

    guard let counterDataBuffer = counterDataBuffer else {
        return nil
    }

    let range = 0..

```
(id) resolveSampleBuffer:(id)sampleBuffer
                      withBlitEncoder:(id)blitEncoder
              toBufferWithStorageMode:(MTLResourceOptions)storageMode
{
    NSUInteger counterBufferLength = self.sampleCount * sizeof(MTLCounterResultTimestamp);
    id counterDataBuffer = [sampleBuffer.device newBufferWithLength: counterBufferLength
                                                                       options: storageMode];

    if (nil == counterDataBuffer) {
        return nil;
    }

    NSRange range = NSMakeRange(0, self.sampleCount);

    [blitEncoder resolveCounters:sampleBuffer
                         inRange:range
               destinationBuffer:counterDataBuffer
               destinationOffset:0];

    if (storageMode & MTLStorageModeManaged) {
        [blitEncoder synchronizeResource:counterDataBuffer];
    }

    return counterDataBuffer;
}
```

### Cast the Counter Sample’s Data to a Result Type

Your app can inspect and use the resolved data by casting it to the result type that corresponds to the counter set.

| Counter set names | Counter result types |
|----|----|
| timestamp | MTLCounterResultTimestamp |
| stageUtilization | MTLCounterResultStageUtilization |
| statistic | MTLCounterResultStatistic |

For example, your app can cast the data it resolves from a timestamp counter set as an MTLCounterResultTimestamp array.

- Swift
- Objective-C

```
/// Converts the contents of the counter sample buffer into an array of result timestamps.
func resolveSampleBuffer() {
    ...

    // Convert the contents of the counter sample buffer into the standard data format.
    guard let data = try? counterSampleBuffer.resolveCounterRange(range) else {
        return
    }

    // Declare the destination type for the `Data` instance's contents.
    let timestampSamples: [MTLCounterResultTimestamp]

    // Cast the resolved data into an array of the counter's result type.
    timestampSamples = Array(unsafeUninitializedCapacity: sampleCount) { buffer, initializedCount in
        // Save the size for each counter result timestamp instance.
        let elementSize = MemoryLayout.size

        // Copy the data's bytes into the array's unsafe mutable buffer pointer.
        let bytesCopied = data.copyBytes(to: buffer)

        // Calculate how many complete counter result timestamp elements the method copies.
        initializedCount = bytesCopied / elementSize
    }

    // Check whether the number of samples is correct.
    guard timestampSamples.count == sampleCount else {
        print("Only \(timestampSamples.count) out of \(sampleCount) timestamps resolved.");
        return
    }

    ...
}
```

```
/// Converts the contents of the counter sample buffer into an array of result timestamps.
- (void) resolveSampleBuffer
    ...

    // Convert the contents of the counter sample buffer into the standard data format.
    NSData* data = [self.counterSampleBuffer resolveCounterRange:range];
    ...

    NSUInteger resolvedSampleCount = data.length / sizeof(MTLCounterResultTimestamp);
    if (resolvedSampleCount 

The code example above also checks whether the result type array has the correct number of elements of the counter set for the app.

### Inspect the Information and Check for Error Values

You can also use the result type instances to check whether the GPU stores any error values. The following code example determines whether any of the timestamp samples are equal to `0` or a sentinel error value:

- Swift
- Objective-C

```
/// Converts the contents of the counter sample buffer into an array of result timestamps.
func resolveSampleBuffer() {
    ...

    for (index, sample) in timestampSamples.enumerated() {
        if sample.timestamp == MTLCounterErrorValue {
            print("Timestamp sample \(index + 1) (of \(sampleCount)) has an error value.")
            return
        }

        if sample.timestamp == 0 {
            print("Timestamp sample \(index + 1) (of \(sampleCount)) has a value of zero.")
            return
        }
    }

    ...
}

```

```
/// Converts the contents of the counter sample buffer into an array of result timestamps.
- (void) resolveSampleBuffer
    ...

    // Cast the data's bytes property to the counter's result type.
    MTLCounterResultTimestamp* timestamps = (MTLCounterResultTimestamp *)(data.bytes);

    // Check for invalid values within the (resolved) data from the counter sample buffer.
    for (int index = 0; index 

Any time the GPU encounters a runtime error while sampling a counter, it sets the counter datum to the sentinel value MTLCounterErrorValue.

Note

A GPU typically stores timestamp values from its internal clock. You can convert those timestamps into more meaningful time values, in nanoseconds, with sampleTimestamps() — see Converting GPU Timestamps into CPU Time.

## See Also

### Counter Sample Data Output

struct MTLCounterResultTimestamp

The data structure for storing the data you resolve from a timestamp counter set.

struct MTLCounterResultStatistic

The data structure for storing the data you resolve from a statistic counter set.

struct MTLCounterResultStageUtilization

The data structure for storing the data you resolve from a stage-utilization counter set.

var MTLCounterErrorValue: UInt64

A sentinel value for an entry in a counter sample buffer that indicates the entry’s data is invalid.

