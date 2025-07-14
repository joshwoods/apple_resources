

- Core HID
- HIDDeviceClient
-  HIDDeviceClient.RequestElementUpdate 

Structure

# HIDDeviceClient.RequestElementUpdate

A request to pull the current value from a list of HID elements

macOS 15.0+

``` source
struct RequestElementUpdate
```

## Mentioned in 

Communicating with human interface devices

## Overview

Provide this structure to updateElements(_:timeout:) to request the current values for a list of elements. In most cases, this triggers a get report request to the device for all of the reports containing elements in the provided element list.

## Topics

### Operators

static func == (HIDDeviceClient.RequestElementUpdate, HIDDeviceClient.RequestElementUpdate) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Initializers

init(elements: [HIDElement], pollDevice: Bool)

Creates a request element update.

### Instance Properties

var elements: [HIDElement]

The elements used to request updates.

var hashValue: Int

The hash value.

var pollDevice: Bool

Whether the device should be polled for new updates.

### Instance Methods

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

### Default Implementations

Equatable Implementations

## Relationships

### Conforms To

- Equatable
- HIDElementUpdate
- Hashable
- Sendable

## See Also

### Update element values

func updateElements([any HIDElementUpdate], timeout: Duration?) async -> HIDDeviceClient.HIDElementUpdateResult

Provide new update values for, or request current values from, lists of elements.

struct ProvideElementUpdate

A structure that provides values for a list of HID elements.

struct HIDElementUpdateResult

A class to hold the results of an element update.

