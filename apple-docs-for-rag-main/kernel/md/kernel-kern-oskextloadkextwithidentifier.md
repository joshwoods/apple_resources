

- Kernel
- kern
-  OSKextLoadKextWithIdentifier 

Function

# OSKextLoadKextWithIdentifier

Request that a kext be loaded.

macOS 10.6+

``` source
OSReturn OSKextLoadKextWithIdentifier(const char *kextIdentifier);
```

## Parameters 

`kextIdentifier`  

The bundle identifier of the kext to be loaded.

## Return Value

`kOSReturnSuccess` if the kext was loaded (or was already loaded). `kOSKextReturnDeferred` if the kext was not found and a request was queued to kextd(8). Other return values indicate a failure to load the kext.

## Discussion

If a kext is already in the kernel but not loaded, it is loaded immediately. If it isn't found, an asynchronous load request is made to kextd(8) and `kOSKextReturnDeferred` is returned. There is no general notification or callback mechanism for load requests.

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

OSKextReleaseKextWithLoadTag

Release a loaded kext based on its load tag.

OSKextRequestResource

Requests data from a nonlocalized resource file in a kext bundle on disk.

OSKextResetPgoCounters

OSKextResetPgoCountersLock

OSKextResetPgoCountersUnlock

OSKextRetainKextWithLoadTag

Retain a loaded kext based on its load tag, and enable autounload for that kext.

