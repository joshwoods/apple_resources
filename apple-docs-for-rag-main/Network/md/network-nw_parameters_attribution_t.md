

- Network
-  nw_parameters_attribution_t 

Enumeration

# nw_parameters_attribution_t

The entities that can make a network request.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.0+macOS 10.14+tvOS 12.0+visionOS 1.0+watchOS 6.0+

``` source
enum nw_parameters_attribution_t
```

## Overview

Use one of these values when setting the `attribution` parameter of a network request with the nw_parameters_get_attribution(_:) method. If you don’t set a value, the system assumes nw_parameters_attribution_t.developer.

## Topics

### Request Sources

case developer

A developer-initiated network request.

case user

The user explicitly directs the app to make a network request.

### Initializers

init?(rawValue: UInt8)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Traffic Attribution

Inspecting app activity data

Verify that your app accesses only the user data and network resources that you expect it to access.

Indicating the source of network activity

Control whether the App Privacy Report attributes network traffic to the app or to the user.

func nw_parameters_set_attribution(nw_parameters_t, nw_parameters_attribution_t)

Sets a flag that indicates whether the network request originates from the developer or the user.

func nw_parameters_get_attribution(nw_parameters_t) -> nw_parameters_attribution_t

Gets a flag that indicates whether the network request originates from the developer or the user.

