

- Bundle Resources
- Entitlements
-  com.apple.developer.kernel.increased-memory-limit 

Property List Key

# com.apple.developer.kernel.increased-memory-limit

A Boolean value that indicates whether core features of your app may perform better with a higher memory limit on supported devices.

iOS 15.0+iPadOS 15.0+

## Details 

Type  

boolean

## Discussion

Add this entitlement to your app to inform the system that some of your app’s core features may perform better by exceeding the default app memory limit on supported devices. If you use this entitlement, make sure your app still behaves correctly if additional memory isn’t available.

Note

An increased memory limit is only available on some device models. Call the os_proc_available_memory function to determine the amount of memory available. Higher memory use can affect system performance.

## See Also

### Memory

Extended Virtual Addressing Entitlement

A Boolean value that indicates whether the app may access an extended address space.

**Key:** com.apple.developer.kernel.extended-virtual-addressing

