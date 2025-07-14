

- Metal
- GPU Devices and Work Submission
-  Multi-GPU Systems 

API Collection

# Multi-GPU Systems

Locate and work with internal and external GPUs and their displays, video memory, and performance tradeoffs.

## Overview

Your app can submit work to any or all of the GPUs of a system that supports multiple GPUs. For example, every Mac notebook, such as a MacBook Pro, has an internal GPU, but some have two.

A Mac may have a Thunderbolt connection to an external GPU and its displays.

Some systems may have even more complicated arrangements of internal and multiple external GPUs and displays.

For more information about Mac configurations with GPUs and displays, see Assessing Multi-GPU and Multi-Display Setups on an Intel-Based Mac.

Start by locating all GPUs in a system and identifying their types (see Finding Multiple GPUs on an Intel-based Mac). Alternatively, you can locate a specific GPU that’s driving a display (see Getting the GPU that Drives a View’s Display).

When selecting a GPU, consider its memory bandwidth and the storage mode options for its memory resources (see Adjusting for GPU Memory Bandwidth Tradeoffs).

For examples of how to use external GPUs in your graphics rendering or compute processing workflows, see the following:

- Selecting Device Objects for Graphics Rendering

- Selecting Device Objects for Compute Processing

For more information about external GPU configurations, see Use an external graphics processor with your Mac.

Note

The system may gain or lose an external GPU at any time (see Handling External GPU Additions and Removals).

## Topics

### Locating GPUs

Finding Multiple GPUs on an Intel-based Mac

Locate, identify, and choose suitable GPUs for your app.

Getting the GPU that Drives a View’s Display

Keep up to date with the optimal device for your display.

func MTLCopyAllDevices() -> [any MTLDevice]

Returns an array of all the Metal device instances in the system.

func MTLCopyAllDevicesWithObserver(handler: MTLDeviceNotificationHandler) -> (devices: [any MTLDevice], observer: NSObject)

Returns an array of all the Metal GPU devices in the system and registers a notification handler that Metal calls when the device list changes.

func MTLRemoveDeviceObserver(any NSObjectProtocol)

Removes a registered observer of device notifications.

func CGDirectDisplayCopyCurrentMetalDevice(_ display: CGDirectDisplayID) -> (any MTLDevice)?

Returns the GPU device instance that’s currently driving a display.

typealias MTLDeviceNotificationHandler

A Swift closure or an Objective-C block that Metal calls when the system adds or removes a GPU device.

struct MTLDeviceNotificationName

A notification that represents a change to a GPU device in the system.

### Selecting GPUs

Adjusting for GPU Memory Bandwidth Tradeoffs

Choose a suitable GPU and memory storage mode for tasks based on that GPU’s memory bandwidth on a Mac.

Assessing Multi-GPU and Multi-Display Setups on an Intel-Based Mac

Learn the possible GPU and display configurations for a Mac and their limitations.

Selecting Device Objects for Graphics Rendering

Switch dynamically between multiple GPUs to efficiently render to a display.

Selecting Device Objects for Compute Processing

Switch dynamically between multiple GPUs to efficiently execute a compute-intensive simulation.

### Working with External GPUs

Handling External GPU Additions and Removals

Register and respond to external GPU notifications that a person initiates.

Transferring Data Between Connected GPUs

Use high-speed connections between GPUs to transfer data quickly.

## See Also

### Locating and Inspecting a GPU Device

Getting the Default GPU

Select the system’s default GPU device on which to run your Metal code.

Detecting GPU Features and Metal Software Versions

Use the device object’s properties to determine how you perform tasks in Metal.

func MTLCreateSystemDefaultDevice() -> (any MTLDevice)?

Returns the device instance Metal selects as the default.

protocol MTLDevice

The main Metal interface to a GPU that apps use to draw graphics and run computations in parallel.

