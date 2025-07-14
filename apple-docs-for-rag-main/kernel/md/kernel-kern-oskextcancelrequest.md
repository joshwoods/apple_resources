

- Kernel
- kern
-  OSKextCancelRequest 

Function

# OSKextCancelRequest

Cancels a pending user-space kext request without invoking the callback.

macOS 10.6+

``` source
OSReturn OSKextCancelRequest(OSKextRequestTag requestTag, void **contextOut);
```

## Parameters 

`requestTag`  

A tag identifying a pending request.

`contextOut`  

If non-`NULL`, filled with the context pointer originally passed with the request.

## Return Value

`kOSReturnSuccess` if the request is successfully canceled. `kOSKextReturnNotFound` if `requestTag` does not identify any pending request. Other `OSKextReturn...` errors are possible.

## Discussion

This function cancels a pending request if it exists, so that its callback will not be invoked. It returns in `contextOut` the context pointer used to create the request so that any resources allocated for the request can be cleaned up.

Kexts do not need to cancel outstanding requests in their module stop functions; when a kext is unloaded, all pending request callbacks are invoked with a result of `kOSKextReturnTimeout` before the stop function is called.

## See Also

### kext

kext_alloc

kext_alloc_init

kext_free

kext_request

kextd_ping

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

