

- Core HID
- HIDDeviceClient
-  HIDDeviceClient.UnsafeProperty 

Structure

# HIDDeviceClient.UnsafeProperty

A wrapper around an object to facilitate working with subscripts.

macOS 15.0+

``` source
struct UnsafeProperty
```

## Overview

Note that this is unchecked Sendable, and therefore unsafe. The contained object is NOT guaranted to be concurrency safe.

## Topics

### Instance Properties

let unsafeObject: AnyObject

An object may not be safe to use concurrently.

## Relationships

### Conforms To

- Sendable

