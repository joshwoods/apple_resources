

- Kernel
- kern
-  OSKextRequestResource 

Function

# OSKextRequestResource

Requests data from a nonlocalized resource file in a kext bundle on disk.

macOS 10.6+

``` source
OSReturn OSKextRequestResource(const char *kextIdentifier, const char *resourceName, OSKextRequestResourceCallback callback, void *context, OSKextRequestTag *requestTagOut);
```

## Parameters 

`kextIdentifier`  

The CFBundleIdentifier of the kext from which to read the file.

`resourceName`  

The name of the resource file to read.

`callback`  

A pointer to a callback function; the address must be within a currently-loaded kext.

`context`  

A pointer to arbitrary run-time data that will be passed to the callback when it is invoked. May be `NULL`.

`requestTagOut`  

If non-`NULL`, filled on success with a tag identifying the pending request (or on failure with `kOSKextRequestTagInvalid`; can be used with OSKextCancelRequest.

## Return Value

`kOSReturnSuccess` if the request is successfully queued. `kOSKextReturnInvalidArgument` if `kextIdentifier` or `resourceName` or if `callback` is not an address within a loaded kext executable. `kOSKextReturnStopping` if an unload attempt is being made on the kext containing `callback`. Other `OSKextReturn...` errors are possible.

## Discussion

This function queues an asynchronous request to the user-space kext daemon kextd(8); requests for resources early in system startup will not be fulfilled until that daemon starts. Requests made by a kext while that kext is loading (specifically in the kext's module start routine) will not be fulfilled until after the start routine returns and the kext is completely loaded. Kexts requesting resources should be sure to perform appropriate locking in the callback function.

Kext resources are stored in the kext's on-disk bundle under the Resources subdirectory. See Bundle Programming Guide for an overview of bundle structure. The localization context of the kext daemon (namely that of the superuser) will be used in retrieving resources; kext resources intended for use in the kernel should generally not be localized.

`callback` is guaranteed to be invoked except when:

- OSKextCancelRequest is used to cancel the request. In this case the kext gets the `context` pointer and can clean it up.

- The request is made during a kext's module start routine and the start routine returns an error. In this case, callbacks cannot be safely invoked, so the kext should clean up all request contexts when returning the error from the start routine.

Kexts with pending requests are not subject to autounload, but requests are subject to timeout after a few minutes. If that amount of time passes with no response from user space, `callback` is invoked with a result of. `kOSKextReturnTimeout`.

Kexts that are explicitly unloaded have all pending request callbacks invoked with a result of `kOSKextReturnStopping`. The kext must handle these callbacks, even if its stop routine will prevent unloading. If the kext does prevent unloading, it can reissue resource requests outside of the stop function.

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

OSKextReleaseKextWithLoadTag

Release a loaded kext based on its load tag.

OSKextResetPgoCounters

OSKextResetPgoCountersLock

OSKextResetPgoCountersUnlock

OSKextRetainKextWithLoadTag

Retain a loaded kext based on its load tag, and enable autounload for that kext.

