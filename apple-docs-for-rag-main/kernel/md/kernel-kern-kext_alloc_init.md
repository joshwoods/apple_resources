

- Kernel
- kern
-  kext_alloc_init 

Function

# kext_alloc_init

macOS 15.0+

``` source
void kext_alloc_init(void);
```

## See Also

### kext

kext_alloc

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

OSKextReleaseKextWithLoadTag

Release a loaded kext based on its load tag.

OSKextRequestResource

Requests data from a nonlocalized resource file in a kext bundle on disk.

OSKextResetPgoCounters

OSKextResetPgoCountersLock

OSKextResetPgoCountersUnlock

OSKextRetainKextWithLoadTag

Retain a loaded kext based on its load tag, and enable autounload for that kext.

