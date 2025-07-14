

- Kernel
- Kernel Data Types
-  sf_notify_func 

Type Alias

# sf_notify_func

macOS 10.4+

``` source
typedef void (*sf_notify_func)(void *cookie, socket_t so, sflt_event_t event, void *param);
```

## Parameters 

`cookie`  

Cookie value specified when the filter attach was called.

`so`  

The socket the filter is attached to.

`event`  

The type of event that has occurred.

`param`  

Additional information about the event.

## Discussion

sf_notify_func is called to notify the filter of various state changes and other events occuring on the socket.

