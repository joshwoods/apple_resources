

- Core HID
- HIDDeviceClient
-  HIDDeviceClient.HIDElementUpdateResult 

Structure

# HIDDeviceClient.HIDElementUpdateResult

A class to hold the results of an element update.

macOS 15.0+

``` source
struct HIDElementUpdateResult
```

## Overview

This class is received as the return value from updateElements(_:timeout:). The results of the transactions can be received by subscripting the results object with HIDDeviceClient.ProvideElementUpdate and HIDDeviceClient.RequestElementUpdate originally passed to updateElements(_:timeout:).

For an example, see updateElements(_:timeout:).

## Topics

### Subscripts

subscript(HIDDeviceClient.ProvideElementUpdate) -> Result&lt;Void, any Error>?

Receive the result of a element update.

subscript(HIDDeviceClient.RequestElementUpdate) -> Result&lt;[HIDElement.Value], any Error>?

Receive the result of a request element update.

## Relationships

### Conforms To

- Sendable

## See Also

### Update element values

func updateElements([any HIDElementUpdate], timeout: Duration?) async -> HIDDeviceClient.HIDElementUpdateResult

Provide new update values for, or request current values from, lists of elements.

struct RequestElementUpdate

A request to pull the current value from a list of HID elements

struct ProvideElementUpdate

A structure that provides values for a list of HID elements.

