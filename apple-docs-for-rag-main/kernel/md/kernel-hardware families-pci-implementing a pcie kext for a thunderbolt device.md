

- Kernel
- Hardware Families
- PCI
-  Implementing a PCIe Kext for a Thunderbolt Device 

Article

# Implementing a PCIe Kext for a Thunderbolt Device

Create an IOKit driver to support Thunderbolt devices that implement features not supported in PCIDriverKit, such as wireless networking or audio.

## Overview

If you manufacture Thunderbolt devices, create a custom driver only when your device contains unique features that require additional support. Apple supplies drivers for many standard protocols and device types, alleviating the need for you to create custom drivers in some cases. However, if your Thunderbolt device contains PCIe endpoints that require additional support, create a custom PCIe driver to support those endpoints.

Create the PCIe driver for your Thunderbolt device using PCIDriverKit whenever possible. DriverKit extensions run in user space and require less effort to develop, debug, and deploy. However, PCIDriverKit may not be an option in all cases. If your device supports wireless networking or audio, or if it requires specific kernel resources, you must create your driver as an IOKit kernel extension.

Kernel extensions run in the kernel process space of the target Mac computer using the native architecture. To support both Apple silicon and Intel-based Mac computers, build your driver as a universal binary. For the most part, your driver code is identical on both Apple silicon and Intel-based Macs. However, if you’re updating a driver you previously built only for Intel-based Macs, you may need to update your code to correctly handle:

- Pointer authentication

- Memory architecture differences between Apple silicon and Intel-based Macs

- Kernel integrity protection (KIP) restrictions

For basic information about building kernel extensions, see Kernel Extension Programming Topics. For information about how to develop drivers using PCIDriverKit, see Creating Custom PCIe Drivers for Thunderbolt Devices.

### Implement Your Driver Life Cycle Normally

The life cycle of a kernel extension in macOS 11 remains unchanged from previous versions of macOS. In particular, the system loads your custom IOService subclass, and calls its init and Start methods. Use the `init` method to allocate your driver’s data structures. Use the `Start` method to configure your hardware, install event handlers, and prepare your driver to handle requests. When your driver is no longer needed, the system calls the corresponding Stop and free methods to release any driver-related resources.

For information about how to implement your driver life cycle, see IOKit Fundamentals.

### Access Memory Using DMA Commands

Thunderbolt devices access system memory through a system-provided I/O memory management unit (IOMMU). On Intel-based Mac computers, the system provides a single IOMMU and gives all devices a shared view of system memory. On Macs with Apple silicon, the system gives each device its own IOMMU. Always implement your driver as if it has its own IOMMU, and never assume you have a shared view of system memory.

To transfer memory correctly on all types of Macs, use an IODMACommand object configured with the kMapped option. Typically, you create one or more of these objects at startup and reuse them multiple times. To create one, fetch the IOMapper object associated with your driver’s provider object and pass it to the appropriate `IODMACommand` creation function. For example, the following code creates a command object for 64-bit transfers with several standard transfer options.

IOMapper *mapper = IOMapper::copyMapperForDevice(provider);
IODMACommand *dmaCommand = 
     IODMACommand::withSpecification(kIODMACommandOutputHost64, 
              64,      // 64-bit transfers
              0,       // Unlimited segment sizes
              (IODMACommand::MappingOptions)(IODMACommand::kMapped),
              0,       // No maximum transfer size
              1,       // 1-byte alignment
              mapper, 
              NULL);

When you are ready to transfer data to or from your device, create a new memory descriptor to handle the transferred data. Configure the descriptor with the kIODirectionIn direction to read data from the device into memory, or configure it with the kIODirectionOut direction to send data from memory out to the device. Assign the memory descriptor to your `IODMACommand` object using its setMemoryDescriptor method, the default options for which begin the transfer operation immediately.

Note

Calls to the getPhysicalSegment method of `IOMemoryDescriptor` fail on Apple silicon. When updating older kernel extensions to support Apple silicon, replace all calls to that method with IODMACommand objects.

### Add Thunderbolt Support to Your Driver’s Personality Data

When it detects new hardware, the system must find an appropriate set of drivers to manage that hardware. It does so by comparing the hardware details to information found in the `kIOKitPersonalitiesKey` key of each driver’s `Info.plist` file, and identifying the drivers that best match the hardware. For example, a driver might match only against devices from a specific manufacturer, or devices that support only a specific communication protocol.

To indicate that your PCIe driver supports Thunderbolt, include the `IOPCITunnelCompatible` key in your driver’s personality dictionaries. Include this key only if the IOService subclass in the `IOClass` key of that dictionary is able to communicate with your Thunderbolt device. The following example shows the presence of this key in a custom PCI driver.

&lt;key>MyDriverKitDriver&lt;/key>
&lt;dict>
    &lt;key>CFBundleIdentifier&lt;/key>
    &lt;string>$(PRODUCT_BUNDLE_IDENTIFIER)&lt;/string>
    &lt;key>CFBundleIdentifierKernel&lt;/key>
    &lt;string>com.apple.kpi.iokit&lt;/string>
    &lt;key>IOClass&lt;/key>
    &lt;string>IOUserService&lt;/string>
    &lt;key>IOPCIPauseCompatible&lt;/key>
    &lt;true/>
    &lt;key>IOPCIPrimaryMatch&lt;/key>
    &lt;string>0x0000ABCD&amp;amp;0x0000FFFF&lt;/string>
    &lt;key>IOPCITunnelCompatible&lt;/key>
    &lt;true/>
    &lt;key>IOProviderClass&lt;/key>
    &lt;string>IOPCIDevice&lt;/string>
    &lt;key>IOResourceMatch&lt;/key>
    &lt;string>IOKit&lt;/string>
    &lt;key>IOUserClass&lt;/key>
    &lt;string>MyPCIDriverKitDriverClassName&lt;/string>
    &lt;key>IOUserServerName&lt;/key>
    &lt;string>com.apple.MyDriverKitDriver&lt;/string>
&lt;/dict>

When a device supports Thunderbolt, the system adds the `IOPCITunnelled` property to one of the drivers in the chain and sets the value of that property to true. If you need to know whether the device is a Thunderbolt device, search for this property in your driver code. For example, you might do so before enabling specific features in your code that require Thunderbolt. The following example searches all parent drivers in the global service plane for the property. If the property is present, the code checks its value to determine whether the device is a Thunderbolt device.

bool isThunderboltEnabled = false;
OSContainer* container = NULL;
if (SearchProperty(&quot;IOPCITunnelled&quot;, &quot;IOService&quot;, kIOServiceSearchPropertyParents, &amp;container) == kIOReturnSuccess)
{
   OSBoolean* boolVar = OSDynamicCast(OSBoolean, container);
   if (boolVar != NULL &amp;&amp; boolVar == kOSBooleanTrue)
   {
      // The device supports Thunderbolt.
      isThunderboltEnabled = true;
   }
   OSSafeReleaseNULL(container);
}

### Notify the System of External Storage Devices

Users can disconnect most Thunderbolt devices at any time, but macOS doesn’t allow them to disconnect external storage devices without properly ejecting them. If your PCI driver presents the device as storage to the system, notify the system early in your driver’s start method by setting the `Physical Interconnect Location` property to `External`, as shown in the following example.

// Add the Physical Interconnect Location property to the driver.
OSDictionary* dict = OSDictionary::withCapacity(1);
OSString* externalStr = OSString::withCString(&quot;External&quot;);
dict->setObject(&quot;Physical Interconnect Location&quot;, externalStr);
SetProperties(dict);
OSSafeReleaseNULL(externalStr);
OSSafeReleaseNULL(dict);

Important

Always set the `Physical Interconnect Location` property early in your driver’s start method. Don’t set it after you access the device.

### Avoid Audio Glitches Caused by Power Transitions

The processors in recent Macs have low-power states that reduce the processor speed and voltage when the computer is idle. These low-power states decrease overall power consumption and heat generation on the system, and improve battery life. However, when a power-state transition occurs, the system temporarily stops all PCI bus traffic while it changes the power state of the processor cores. Halting PCI bus traffic can cause audio glitches and other side effects on devices that are sensitive to the added latency.

To mitigate the problems of any added latency, implement the PCIe latency tolerance reporting (LTR) extended capability in your devices according to the PCIe specifications. If your driver supports legacy devices, schedule your driver’s time-critical DMA operations so that occasional delays don’t affect your device. If you’re unable to adjust the schedule of your DMA operations, call the requireMaxBusStall method of your `IOService` subclass at the beginning and end of any time-critical transfers. Before a transfer, call this method with the constant that represents the maximum latency your driver can tolerate. For example, specify `kIOMaxBusStall20usec` to delay bus stalls for 20 microseconds. The system avoids entering low-power states for the specified amount of time. After a transfer, restore the default bus stall time by passing `kIOMaxBusStallNone` to the method.

Important

Call the `requireMaxBusStall` method only if there is no other way to make your device and driver more tolerant of increased memory latency. The method prevents the system from transitioning to lower-power states, which can significantly impact battery life on portable systems. It may also increase system heat, and require device fans to run longer. Overuse of this API may also lead to kernel panics.

Because audio transfers occur only when your audio engine is running, call the `requireMaxBusStall` method in the performAudioEngineStart and performAudioEngineStop methods of `IOAudioEngine`. The following example shows an implementation of these methods that prevents PCI bus stalls for 10 microseconds when a transfer begins, and restores the default bus stall time at the end of the transfer.

/* Header file */
class MyAudioEngine : public IOAudioEngine
{
    /* virtual overrides, custom function, variables, etc... */
public:
    virtual IOReturn performAudioEngineStart();
    virtual IOReturn performAudioEngineStop();
}

/* Implementation file */
IOReturn MyAudioEngine::performAudioEngineStart()
{
    requireMaxBusStall(kIOMaxBusStall10usec);
    return IOAudioEngine::performAudioEngineStart();
}

IOReturn MyAudioEngine::performAudioEngineStop()
{
    // Zero means restore default bus stall time.
    // It&#39;s now safe to go into lowest-power states.
    requireMaxBusStall(kIOMaxBusStallNone);
    return IOAudioEngine::performAudioEngineStop();
}

### Build Your Kernel Extension as a Universal Binary

Build your kernel extension as a universal binary on macOS 11 and later. A universal binary supports both Apple silicon and Intel-based Mac computers.

On Macs with Apple silicon, the kernel is built for the ARM64e architecture, so you must similarly build your kernel extensions for that architecture. The ARM64e architecture enables pointer authentication, a security feature that prevents the unexpected modification of pointers at runtime. For more information about how to support pointer authentication, see Preparing your app to work with pointer authentication.

## See Also

### Devices

IOPCIDevice

An IOService class representing a PCI device.

Deprecated

IOAGPDevice

An IOService class representing an AGP primary device.

Deprecated

