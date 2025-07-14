

- Kernel
- kern
-  kextd_ping 

Function

# kextd_ping

macOS 10.6+

``` source
kern_return_t kextd_ping(mach_port_t server);
```

## See Also

### kext

kext_alloc

kext_alloc_init

kext_free

kext_request

OSKextCancelRequest

Cancels a pending user-space kext request without invoking the callback.

OSKextGetCurrentIdentifier

Returns the CFBundleIdentifier for the calling kext as a C string.

OSKextGetCurrentLoadTag

Returns the run-time load tag for the calling kext as an `OSKextLoadTag`.

OSKextGetCurrentVersionString

Returns the CFBundleVersion for the calling kext as a C string.

OSKextGrabPgoData

OSKextLoadKextWithIdentifier

Request that a kext be loaded.

OSKextReleaseKextWithLoadTag

Release a loaded kext based on its load tag.

OSKextRequestResource

Requests data from a nonlocalized resource file in a kext bundle on disk.

OSKextResetPgoCounters

OSKextResetPgoCountersLock

OSKextResetPgoCountersUnlock

OSKextRetainKextWithLoadTag

Retain a loaded kext based on its load tag, and enable autounload for that kext.

