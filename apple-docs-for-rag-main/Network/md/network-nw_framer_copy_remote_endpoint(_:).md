

- Network
-  nw_framer_copy_remote_endpoint(\_:) 

Function

# nw_framer_copy_remote_endpoint(\_:)

Accesses the remote endpoint of the connection in which your protocol is running.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
func nw_framer_copy_remote_endpoint(_ framer: nw_framer_t) -> nw_endpoint_t
```

## See Also

### Inspecting Instance Properties

func nw_framer_copy_local_endpoint(nw_framer_t) -> nw_endpoint_t

Accesses the local endpoint of the connection in which your protocol is running.

func nw_framer_copy_parameters(nw_framer_t) -> nw_parameters_t

Accesses the parameters of the connection in which your protocol is running.

