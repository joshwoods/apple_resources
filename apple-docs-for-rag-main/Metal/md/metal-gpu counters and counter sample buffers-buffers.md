

- Metal
-  GPU Counters and Counter Sample Buffers 

API Collection

# GPU Counters and Counter Sample Buffers

Retrieve runtime data from a GPU device by sampling one or more of its counters.

## Overview

A GPU *counter* (MTLCounter) is typically a hardware feature that tracks a specific performance metric, such as timestamps before and after an important rendering stage. A *counter set* (MTLCounterSet) is a collection of related counters. A *counter sample buffer* (MTLCounterSampleBuffer) represents the memory where a GPU device stores the data for a specific counter set.

You can retrieve and inspect data from a GPU’s counter set with the following steps:

1.  Inspect which GPU counter sets a GPU device supports (see Confirming which Counters and Counter Sets a GPU Supports).

2.  Make a counter sample buffer to store the data (see Creating a Counter Sample Buffer to Store a GPU’s Counter Data During a Pass).

3.  Instruct the GPU to save the counter set data to the buffer during a pass or an immediate mode command (see Sampling GPU Data into Counter Sample Buffers).

4.  Transform the counter set data into a standard type (see Converting a GPU’s Counter Data into a Readable Format).

If you’re sampling data from a timestamp counter set (timestamp), you may need to convert the timestamps from the GPU’s clock to the CPU’s clock. See Converting GPU Timestamps into CPU Time for more information.

## Topics

### Counters and Counter Sets

Confirming which Counters and Counter Sets a GPU Supports

Check whether a GPU produces the runtime performance data you want to sample.

protocol MTLCounterSet

A collection of individual counters a GPU device supports for a counter set.

struct MTLCommonCounterSet

The name of a specific counter set that a GPU device can support.

protocol MTLCounter

An individual counter a GPU device lists within one of its counter sets.

struct MTLCommonCounter

The name of a specific counter that can appear in a GPU device’s counter sets.

### Counter Sample Buffers

Creating a Counter Sample Buffer to Store a GPU’s Counter Data During a Pass

Make a buffer that provides a place for a GPU to save its runtime performance metrics as it runs a pass.

class MTLCounterSampleBufferDescriptor

A group of properties that configures the counter sample buffers you create with it.

protocol MTLCounterSampleBuffer

A specialized memory buffer that stores a GPU’s counter set data.

Sampling GPU Data into Counter Sample Buffers

Retrieve a GPU’s counter data at a time the GPU supports.

var MTLCounterDontSample: Int

A sentinel value that instructs an encoder to skip sampling a counter as the GPU runs the encoder’s pass.

### Counter Sample Data Output

Converting a GPU’s Counter Data into a Readable Format

Inspect and use the data within a GPU’s counter sample buffer by resolving it into a standard format.

struct MTLCounterResultTimestamp

The data structure for storing the data you resolve from a timestamp counter set.

struct MTLCounterResultStatistic

The data structure for storing the data you resolve from a statistic counter set.

struct MTLCounterResultStageUtilization

The data structure for storing the data you resolve from a stage-utilization counter set.

var MTLCounterErrorValue: UInt64

A sentinel value for an entry in a counter sample buffer that indicates the entry’s data is invalid.

### Timestamp Data

Converting GPU Timestamps into CPU Time

Correlate GPU events with CPU timelines by calculating the CPU time equivalents for GPU timestamps.

typealias MTLTimestamp

The number of nanoseconds for a point in absolute time or Mach absolute time.

### Counter Sample Buffer Errors

struct MTLCounterSampleBufferError

The error codes that indicate why a GPU driver can’t create a counter sample buffer.

## See Also

### Developer Tools

Metal developer workflows

Locate and fix issues related to your app’s use of the Metal API and GPU functions.

Metal debugger

Debug and profile your Metal workload with a GPU trace.

Improving your game’s graphics performance and settings

Fix performance glitches and develop default settings for smooth experiences on Apple platforms using the powerful suite of Metal development tools.

Capturing Metal Commands Programmatically

Invoke Metal’s frame capture from your app, then save the resulting GPU trace to a file or view it in Xcode.

Supporting Simulator in a Metal app

Configure alternative render paths in your Metal app to enable running your app in Simulator.

Analyzing the memory usage of your Metal app

Keep your app alive in the background by managing its memory footprint.

Analyzing the performance of your Metal app

Ensure consistent, smooth rendering by profiling your app’s frame time.

Developing Metal apps that run in Simulator

Prototype and test your Metal apps in Simulator.

Metal Debugging Types

Create capture managers and capture scopes, and review a GPU device’s log after it runs a command buffer.

