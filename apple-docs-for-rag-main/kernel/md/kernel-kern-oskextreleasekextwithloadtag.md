

- Kernel
- kern
-  OSKextReleaseKextWithLoadTag 

Function

# OSKextReleaseKextWithLoadTag

Release a loaded kext based on its load tag.

macOS 10.6+

``` source
OSReturn OSKextReleaseKextWithLoadTag(OSKextLoadTag loadTag);
```

## Parameters 

`loadTag`  

The load tag of the kext to be released. See OSKextGetCurrentLoadTag.

## Return Value

`kOSReturnSuccess` if the kext was released. `kOSKextReturnNotFound` if the kext was not found. `kOSKextReturnInvalidArgument` if `loadTag` is `kOSKextInvalidLoadTag`.

## Discussion

The kext should have been retained previously via OSKextRetainKextWithLoadTag.

This function schedules an autounload scan for all kexts. When that scan occurs, if a kext has autounload enabled, it will be unloaded if there are no outstanding references to it and there are no instances of its Libkern C++ classes (if any).

Kexts that define subclasses of IOService have autounload enabled automatically. Other kexts can use the reference count to manage automatic unload without having to define and create Libkern C++ objects. For example, a filesystem kext can be retained whenever a new mount is created, and released when a mount is removed. When the last mount is removed, the kext will be unloaded after a brief delay.

While the autounload scan takes place after a delay of at least a minute, a kext that manages its own reference counts for autounload should be prepared to have its module stop function called even while the function calling this function is still running.

A kext can get its own load tag using the OSKextGetCurrentLoadTag.

Kexts should not retain and release other kexts; linkage references are accounted for internally.

## See Also

### kext

kext_alloc

kext_alloc_init

kext_free

kext_request

kextd_ping

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

OSKextRequestResource

Requests data from a nonlocalized resource file in a kext bundle on disk.

OSKextResetPgoCounters

OSKextResetPgoCountersLock

OSKextResetPgoCountersUnlock

OSKextRetainKextWithLoadTag

Retain a loaded kext based on its load tag, and enable autounload for that kext.

