

- Core Services
- Apple Events
-  AERemoteProcessResolverContext 

Structure

# AERemoteProcessResolverContext

Supplied as a parameter when performing asynchronous resolutionof remote processes.

Mac Catalyst 13.0+macOS 10.3+

``` source
struct AERemoteProcessResolverContext
```

## Overview

When you call AERemoteProcessResolverScheduleWithRunLoop(_:_:_:_:_:) forasynchronous resolution, you supply a reference to a structure ofthis type, along with a reference to a callback routine, definedby AERemoteProcessResolverCallback.The context is copied and the info pointer retained. When the callbackis made, the info pointer is passed to the callback.

## Topics

### Initializers

init()

init(version: CFIndex, info: UnsafeMutableRawPointer!, retain: CFAllocatorRetainCallBack!, release: CFAllocatorReleaseCallBack!, copyDescription: CFAllocatorCopyDescriptionCallBack!)

### Instance Properties

var copyDescription: CFAllocatorCopyDescriptionCallBack!

A prototype for a function callback that providesa description of the specified data. Called on the info pointer.This field may be `NULL`.

var info: UnsafeMutableRawPointer!

A pointer to arbitrary information. The pointeris retained and passed to the callback, allowing you to provideinformation to that routine.

var release: CFAllocatorReleaseCallBack!

A prototype for a function callback that releasesthe specified data. Called on the info pointer. This field may be `NULL`.

var retain: CFAllocatorRetainCallBack!

A prototype for a function callback that retainsthe specified data. Called on the info pointer. This field may be `NULL`.

var version: CFIndex

This should be set to zero (0).

