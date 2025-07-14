

- Metal
- Resource Fundamentals
-  Reducing the Memory Footprint of Metal Apps 

Article

# Reducing the Memory Footprint of Metal Apps

Learn best practices for using memory efficiently in iOS and tvOS.

## Overview

Efficient memory usage is a critical consideration for resource-intensive Metal apps in iOS and tvOS. Create apps so they use as little memory as possible, making more memory available for other apps and system services.

iOS and tvOS monitor your app’s total memory usage at runtime, and if the amount exceeds a predetermined limit, the system terminates your app. This limit varies by device model, so test your app on all supported devices.

### Optimize Memory Usage in Your Metal App

Here are some tips to understand how your Metal app is using memory, and best practices to reduce memory usage.

**Use Xcode 11 to measure memory consumption.** Build your app with the iOS or tvOS SDK, then use Xcode Memory Report to observe your app’s total memory footprint during execution. See Gathering information about memory use for more information about Xcode Memory Report.

**Use these tools to gain a deeper understanding of your app’s memory footprint.**

- Take an Instruments trace and look at the Metal Resource Allocations Instrument, which is part of the Metal System Trace template. For more information on working with the Metal Resource Allocations Instrument, see Delivering Optimized Metal Apps and Games.

- Use `Debugging Tools` to capture a GPU trace. Then use the Memory view to get a visual representation of all of a frame’s GPU resources and a table of properties for each resource. See Delivering Optimized Metal Apps and Games for detailed information about the Memory view.

- Observe and take action on suggestions highlighted in the Memory insights section of the GPU trace summary. See Gain insights into your Metal app with Xcode 12 for more information on Memory insights.

- Use the memory graph tool to help identify leaks and abandoned memory. See Memory Graph Debugging for more information.

- Query the amount of memory available to your app at runtime using the os_proc_available_memory API to help you identify memory spikes.

**Make your assets as small as possible.** Avoid loading a large resource when a smaller one works. Use compressed texture formats. Load lower-resolution textures when running on memory-constrained devices. Consider reducing the fidelity of 3D models and compressing per-vertex data.

**Simplify memory-intensive special effects.** Some effects, like shadows or motion blur, require large offscreen buffers for temporary image data. Consider lowering the resolution of these image buffers or applying fewer effects when running on memory-constrained devices.

**Avoid loading unused resources.** Xcode can help you identify Metal objects that aren’t in use. Use Metal Debugger to get a GPU trace. Then navigate to the Memory view, and select the Unused filter.

**Designate resources as volatile when possible.** Use MTLPurgeableState.volatile and setPurgeableState(_:) for textures and buffers the operating system can safely discard under low-memory conditions, and be subsequently recreated or reloaded by your app as needed. This design means your app keeps a cache of idle resources in memory but doesn’t count them toward the memory limit.

**Use memoryless texture storage for temporary-render targets.** MTLStorageMode.memoryless avoids allocating regular system memory, allowing apps to store the contents of temporary render targets directly in tile memory on the GPU.

**Use Metal resource heaps.** Using MTLHeap, your app can have Multiple Metal resources backed by the same memory allocation. For example, use resource heaps when transient resources are produced and consumed for each frame but aren’t all used together. Those not used together share the same memory, backed by a heap.

### Additional Resources

The WWDC video Gain insights into your Metal app with Xcode 12 provides additional information about the latest memory-debugging tools and best practices to help you optimize the memory footprint of your Metal apps and games.

## See Also

### Resource Management

Setting Resource Storage Modes

Set a storage mode that defines the memory location and access permissions of a resource.

Choosing a Resource Storage Mode for Apple GPUs

Select an appropriate storage mode for your textures and buffers on Apple GPUs.

Choosing a Resource Storage Mode for Intel and AMD GPUs

Select an appropriate storage mode for your textures and buffers on AMD and Intel GPUs.

Copying Data to a Private Resource

Use a blit command encoder to copy buffer or texture data to a private resource.

Synchronizing a Managed Resource in macOS

Manually synchronize memory for a Metal resource in apps.

Transferring Data Between Connected GPUs

Use high-speed connections between GPUs to transfer data quickly.

