

- Kernel
- Kernel Enumerations
- Anonymous
-  sock_evt_shutdown 

Enumeration Case

# sock_evt_shutdown

macOS 10.12+

``` source
sock_evt_shutdown = 6
```

## Discussion

The read and or write side(s) of the connection have been shutdown. The param will point to an integer that indicates the direction that has been shutdown. See 'man 2 shutdown' for more information.

