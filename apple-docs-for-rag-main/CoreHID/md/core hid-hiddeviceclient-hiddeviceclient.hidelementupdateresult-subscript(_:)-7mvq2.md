

- Core HID
- HIDDeviceClient
- HIDDeviceClient.HIDElementUpdateResult
-  subscript(\_:) 

Instance Subscript

# subscript(\_:)

Receive the result of a request element update.

macOS 15.0+

``` source
subscript(originalRequest: HIDDeviceClient.RequestElementUpdate) -> Result? { get }
```

## Parameters 

`originalRequest`  

A request that was initially passed to updateElements(_:timeout:).

## Return Value

The result for the specified request which contains a list of updated HIDElement.Value objects. Access the results using get().

## Overview

For an example, see updateElements(_:timeout:).

