

- Metal
- GPU Devices and Work Submission
- Multi-GPU Systems
-  Adjusting for GPU Memory Bandwidth Tradeoffs 

Article

# Adjusting for GPU Memory Bandwidth Tradeoffs

Choose a suitable GPU and memory storage mode for tasks based on that GPU’s memory bandwidth on a Mac.

## Overview

GPU memory *bandwidth* is a measure of the data transfer speed between a GPU and the system across a bus, such as PCI Express (PCIe) or Thunderbolt. It’s important to consider the bandwidth of each GPU in a system when developing your high-performance Metal apps. A GPU that’s powerful on its own may not be the optimal choice for certain tasks if it has a relatively low bandwidth connection to the system.

### Consider How a GPU Connects to the System

A GPU’s bandwidth largely depends on the bus that connects it to a system:

- An *external* GPU connects to a system though an external Thunderbolt 3 bus.

- A *discrete* GPU is a built-in GPU that has video memory (separate memory that only the GPU can access) and connects to a system through an internal PCIe bus.

- An *integrated* GPU is a built-in GPU that uses system memory and shares the bus with the CPU.

A discrete GPU’s PCIe bus can have 8 or 16 memory lanes — or PCIe x4 or PCIe x16, respectively — depending on the GPU and Mac model. Transferring data between the system and an external GPU can take more time than with a built-in GPU because external GPUs typically have a lower bandwidth connection, such as Thunderbolt 3.

Additionally, transferring data from one GPU to another can be even more expensive because the system can’t transfer data directly between GPUs. Instead, the process typically requires copying data to system memory before copying it again to the destination GPU.

### Select the Appropriate Storage Mode for Your Resources

You can minimize the bandwidth costs — the number of data transfers across a bus — by selecting an appropriate storage mode for your app’s resources. For more information about selecting a storage mode for specific GPUs, see Choosing a Resource Storage Mode for Apple GPUs and Choosing a Resource Storage Mode for Intel and AMD GPUs. Metal uses a resource’s storage mode to determine which memory location to save it in. The storage mode options for a resource include the following:

MTLStorageMode.shared  
Shared resources reside in system memory and are slow to access for discrete and external GPUs.

MTLStorageMode.private  
Private resources reside in video memory and are fast to access for discrete and external GPUs.

MTLStorageMode.managed  
Managed resources reside in both system and video memory (dual copies) and are fast to access for discrete and external GPUs.

Discrete and external GPUs have the highest data transfer costs when they access a shared resource because their access to system memory is relatively slow.

Private resources have the lowest data transfer costs with discrete and external GPUs because their exclusive access to video memory is relatively fast.

Managed resources can have modest data transfer costs for discrete and external GPUs. The CPU (and an integrated GPU) have quick access to the copy in system memory, and the other GPUs have quick access to the copy in their video memory.

You can keep the copies in sync by efficiently running sparse blit operations (see Synchronizing a Managed Resource in macOS).

### Render a Drawable on the Same GPU That Drives the Destination Display

In Metal, a *drawable*, represented by MTLDrawable, is a type that bridges Metal and Core Animation. Each drawable contains a texture that your apps can render with Metal and then present on a device’s display using Core Animation.

Presenting a drawable on a display can have significant bandwidth costs if the drawable belongs to a GPU that doesn’t drive the display. Only one GPU can drive a display, whether it’s built in or external, and the fastest path to present a drawable to a display is to render that drawable with the same GPU that drives the display. Otherwise, the system has to transfer the drawable from the GPU that renders it to the GPU that drives the display.

For example, take a Mac that has both a discrete GPU and an external GPU that’s driving an external display. If your app renders a drawable with the discrete GPU, the system has to transfer the drawable to the external GPU through the Thunderbolt 3 bus to present it on the external display. You app can avoid this transfer by rendering the drawable with the external GPU because it’s also driving the drawable’s destination display.

Similarly, Mac systems with multiple built-in GPUs may need to transfer a drawable that one GPU renders if a different GPU drives the destination display. For example, imagine a MacBook Pro with automatic graphics switching is currently driving the built-in display with the integrated GPU. If your app uses the discrete GPU to render a drawable, the system has to transfer the drawable’s contents to the integrated GPU over the internal PCIe bus. Your app can avoid this transfer by rendering the drawable with the integrated GPU when it’s driving the internal display.

## See Also

### Selecting GPUs

Assessing Multi-GPU and Multi-Display Setups on an Intel-Based Mac

Learn the possible GPU and display configurations for a Mac and their limitations.

Selecting Device Objects for Graphics Rendering

Switch dynamically between multiple GPUs to efficiently render to a display.

Selecting Device Objects for Compute Processing

Switch dynamically between multiple GPUs to efficiently execute a compute-intensive simulation.

