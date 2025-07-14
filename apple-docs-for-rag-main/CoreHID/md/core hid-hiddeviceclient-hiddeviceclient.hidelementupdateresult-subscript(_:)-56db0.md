

- Core HID
- HIDDeviceClient
- HIDDeviceClient.HIDElementUpdateResult
-  subscript(\_:) 

Instance Subscript

# subscript(\_:)

Receive the result of a element update.

macOS 15.0+

``` source
subscript(originalRequest: HIDDeviceClient.ProvideElementUpdate) -> Result? { get }
```

## Parameters 

`originalRequest`  

A request that was initially passed to updateElements(_:timeout:).

## Return Value

The result for the specified request that contain Void if successful; otherwise, an error if unsuccessful. Access the results using get().

## Overview

For an example, see updateElements(_:timeout:).

