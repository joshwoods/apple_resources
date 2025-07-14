

- Metal
- GPU Counters and Counter Sample Buffers
-  Converting GPU Timestamps into CPU Time 

Article

# Converting GPU Timestamps into CPU Time

Correlate GPU events with CPU timelines by calculating the CPU time equivalents for GPU timestamps.

## Overview

Sampling runtime data from a GPU can provide a valuable insight to your app’s GPU performance (see Sampling GPU Data into Counter Sample Buffers). GPU timestamps in particular can isolate runtime issues by showing what the GPU is working on relative to what the CPU is doing. However, the timestamp values your app samples from a GPU don’t typically match a CPU’s timestamps because each uses different hardware to measure time. This means you can’t always compare GPU timestamps directly with CPU timestamps.

Your app can convert a GPU’s timestamps to CPU time by sampling both clocks at the same time to establish a common baseline of time. Establish that baseline by sampling both the GPU and CPU clocks at least twice. Typically, apps sample the timestamps at least twice, once before and once after the GPU stores its timestamp data in an MTLCounterSampleBuffer. Your app needs the baseline to accurately convert the GPU’s timestamp data it *resolves* from a counter sample buffer. See Converting a GPU’s Counter Data into a Readable Format for instructions about resolving data within a counter sample buffer.

### Create a Reference Baseline in Time by Sampling the CPU and GPU Timestamps Twice

You can sample timestamps from the GPU and CPU at the same time by calling MTLDevice instance’s sampleTimestamps() method in Swift, or the sampleTimestamps:gpuTimestamp: method in Objective-C.

- Swift
- Objective-C

```
func updateStartTimes(_ device: MTLDevice) {
    // Save the current CPU and GPU times as a baseline.
    let startTimes = device.sampleTimestamps()
    let cpuStart = Double(startTimes.cpu)
    let gpuStart = Double(startTimes.gpu)

    self.cpuStart = cpuStart
    self.gpuStart = gpuStart
}
```

```
- (void) updateStartTimesWithDevice:(id)device {
    // Save the current CPU and GPU times as a baseline.
    MTLTimestamp cpuStartTimestamp = 0;
    MTLTimestamp gpuStartTimestamp = 0;

    [device sampleTimestamps:&cpuStartTimestamp
                gpuTimestamp:&gpuStartTimestamp];

    self.cpuStart = (double)cpuStartTimestamp;
    self.gpuStart = (double)gpuStartTimestamp;
}
```

You can sample the initial timestamps any time before a pass, such as at launch time or when your app creates a command buffer.

Tip

Call sampleTimestamps() sparingly because doing so may trap to the kernel (to read the GPU clock), which can affect your app’s runtime performance.

Calculate the time span by sampling the GPU and CPU timestamps again after the command buffer completes.

- Swift
- Objective-C

```
func updateFinalTimes(_ device: MTLDevice) {
    // Update the final times with the current CPU and GPU times.
    let finalTimes = device.sampleTimestamps()

    cpuTimeSpan = Double(finalTimes.cpu) - cpuStart
    gpuTimeSpan = Double(finalTimes.gpu) - gpuStart
}
```

```
- (void) updateFinalTimesWithDevice:(id)device {
    // Update the final times with the current CPU and GPU times.
    MTLTimestamp cpuFinalTimestamp = 0;
    MTLTimestamp gpuFinalTimestamp = 0;

    [device sampleTimestamps:&cpuFinalTimestamp
                gpuTimestamp:&gpuFinalTimestamp];

    self.cpuTimeSpan = (double)cpuFinalTimestamp - self.cpuStart;
    self.gpuTimeSpan = (double)gpuFinalTimestamp - self.gpuStart;
}
```

The span of time establishes a baseline that your app needs to convert timestamps from a counter sample buffer into real-world time values.

Tip

One good strategy is to sample the timestamps when you create a command buffer, and again inside a completion handler for that command buffer.

For example, the code below samples the GPU and CPU timestamps before and immediately after the GPU runs the command buffer.

- Swift
- Objective-C

```
func configureCommandBuffer(_ commandBuffer: MTLCommandBuffer, frame: Int) {
    guard frame.isMultiple(of: framePollingPeriod) && frame != 0 else {
        return
    }

    timeConverter.updateStartTimes(commandBuffer.device)

    commandBuffer.addCompletedHandler { commandBuffer in
        self.resolveSampleBuffer()
        self.timeConverter.updateFinalTimes(commandBuffer.device)
        self.printVertexAndFragmentDurations(frame)
    }
}
```

```
- (void)  configureCommandBuffer:(id) commandBuffer
                           frame: (NSUInteger)frame;
{
    if (frame % self.framePollingPeriod != 0) {
        return;
    }

    [self.timeConverter updateStartTimesWithDevice:commandBuffer.device];

    [commandBuffer addCompletedHandler:^(id _Nonnull commandBuffer) {
        [self resolveSampleBuffer];
        [self.timeConverter updateFinalTimesWithDevice:commandBuffer.device];
        [self printVertexAndFragmentDurationsForFrame:frame];
    }];
}
```

### Convert GPU Timestamps to CPU Time

Calculate the CPU time equivalent of a GPU timestamp by mathematically converting it using two sets of your app’s reference GPU and CPU timestamps.

Note

The system measures CPU timestamps in nanoseconds.

Convert a GPU timestamp by following these steps:

1.  Subtract the GPU reference starting time from the GPU timestamp.

2.  Divide the difference by the total GPU reference time span.

3.  Multiply the product by the total CPU reference time span.

4.  Add the starting CPU reference time.

- Swift
- Objective-C

```
func absoluteTimeInMicroseconds(timestamp: MTLTimestamp) -> Double {
    guard ready else { return Double.nan }

    // Convert the GPU time to a value within the range [0.0, 1.0].
    let normalizedGpuTime = (Double(timestamp) - gpuStart) / gpuTimeSpan

    // Convert GPU time to CPU time.
    let nanoseconds = (normalizedGpuTime * cpuTimeSpan) + cpuStart

    let microseconds = nanoseconds / 1e3
    return microseconds
}
```

```
- (double) absoluteTimeInMicroseconds:(MTLTimestamp) timestamp {
    // Convert the GPU time to a value within the range [0.0, 1.0].
    double normalizedGpuTime = ((double)timestamp - self.gpuStart);
    normalizedGpuTime /= self.gpuTimeSpan;

    // Convert GPU time to CPU time.
    double nanoseconds = (normalizedGpuTime * self.cpuTimeSpan);
    nanoseconds += self.cpuStart;

    double microseconds = nanoseconds / 1000.0;
    return microseconds;
}
```

The method returns a value in microseconds, but you can convert the value to a unit of time that you prefer.

Similarly, you can calculate the CPU time equivalent between two GPU timestamps by applying the latter calculations to the time span between them.

- Swift
- Objective-C

```
func microsecondsBetween(begin: MTLTimestamp, end: MTLTimestamp) -> Double {
    let timeSpan = Double(end) - Double(begin)

    // Convert GPU time to CPU time.
    let nanoseconds = timeSpan / gpuTimeSpan * cpuTimeSpan

    let microseconds = nanoseconds / 1e3
    return microseconds
}
```

```
- (double) microsecondsBetweenBegin:(MTLTimestamp)begin
                                end:(MTLTimestamp)end {
    double timeSpan = (double)end - (double)begin;

    // Convert GPU time to CPU time.
    double nanoseconds = timeSpan / self.gpuTimeSpan * self.cpuTimeSpan;

    double microseconds = nanoseconds / 1000.0;
    return microseconds;
}
```

This method is useful to show the duration between the beginning and end of an event window. For example, you might use this to see the duration of the vertex and fragment stages of a render pass.

- Swift
- Objective-C

```
func printVertexAndFragmentDurations(_ frame: Int) {
    guard let timestamps = resolvedTimestampSamples else { return }

    print("\n--- Frame \(frame) ---")

    if timestamps.count >= 2 {
        let vertexStart = timestamps[0].timestamp
        let vertexFinish = timestamps[1].timestamp

        let vertexTime = timeConverter.microsecondsBetween(begin: vertexStart,
                                                           end: vertexFinish)

        let roundedTime = String(format: "%.2f", vertexTime)
        print("    Vertex duration:   \(roundedTime) µS")
    }

    if timestamps.count >= 4 {
        let fragmentStart = timestamps[2].timestamp
        let fragmentFinish = timestamps[3].timestamp

        let fragmentTime = timeConverter.microsecondsBetween(begin: fragmentStart,
                                                             end: fragmentFinish)

        let roundedTime = String(format: "%.2f", fragmentTime)
        print("    Fragment duration: \(roundedTime) µS")
    }
}

```

```
- (void) printVertexAndFragmentDurationsForFrame:(NSUInteger)frame
{
    if (nil == self.resolvedTimestampSamples) { return; }

    printf("\n--- Frame %lu ---\n", frame);

    if (self.resolvedTimestampSampleCount >= 2) {
        MTLTimestamp vertexStart = self.resolvedTimestampSamples[0].timestamp;
        MTLTimestamp vertexFinish = self.resolvedTimestampSamples[1].timestamp;

        printf("VS %.2llu\n", vertexStart);
        printf("VF %.2llu\n", vertexFinish);

        double vertexTime;
        vertexTime = [self.timeConverter microsecondsBetweenBegin:vertexStart
                                                              end:vertexFinish];

        printf("    Vertex duration:   %.2f µS\n", vertexTime);
    }

    if (self.resolvedTimestampSampleCount >= 4) {
        MTLTimestamp fragmentStart = self.resolvedTimestampSamples[2].timestamp;
        MTLTimestamp fragmentFinish = self.resolvedTimestampSamples[3].timestamp;

        double fragmentTime;
        fragmentTime = [self.timeConverter microsecondsBetweenBegin:fragmentStart
                                                                end:fragmentFinish];

        printf("    Fragment duration: %.2f µS\n", fragmentTime);
    }
}
```

## See Also

### Timestamp Data

typealias MTLTimestamp

The number of nanoseconds for a point in absolute time or Mach absolute time.

