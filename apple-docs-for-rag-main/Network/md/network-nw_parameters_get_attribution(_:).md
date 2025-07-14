

- Network
-  nw_parameters_get_attribution(\_:) 

Function

# nw_parameters_get_attribution(\_:)

Gets a flag that indicates whether the network request originates from the developer or the user.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
func nw_parameters_get_attribution(_ parameters: nw_parameters_t) -> nw_parameters_attribution_t
```

## Parameters 

`parameters`  

The network parameters to read from.

## Return Value

An indication of whether the network request comes from the developer or from the user.

## See Also

### Traffic Attribution

Inspecting app activity data

Verify that your app accesses only the user data and network resources that you expect it to access.

Indicating the source of network activity

Control whether the App Privacy Report attributes network traffic to the app or to the user.

func nw_parameters_set_attribution(nw_parameters_t, nw_parameters_attribution_t)

Sets a flag that indicates whether the network request originates from the developer or the user.

enum nw_parameters_attribution_t

The entities that can make a network request.

