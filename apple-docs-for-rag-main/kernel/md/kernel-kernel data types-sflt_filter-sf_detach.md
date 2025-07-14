

- Kernel
- Kernel Data Types
- sflt_filter
-  sf_detach 

Instance Property

# sf_detach

Your function for handling detaches from sockets.

macOS 10.6+

``` source
sf_detach_func sf_detach;
```

## See Also

### Fields

sf_handle

A value used to find socket filters by applications. An application can use this value to specify that this filter should be attached when using the SO_NKE socket option.

sf_flags

Indicate whether this filter should be attached to all new sockets or just those that request the filter be attached using the SO_NKE socket option. If this filter utilizes the socket filter extension fields, it must also set SFLT_EXTENDED.

sf_name

A name used for debug purposes.

sf_unregistered

Your function for being notified when your filter has been unregistered.

sf_attach

Your function for handling attaches to sockets.

sf_notify

Your function for handling events. May be null.

sf_data_in

Your function for handling incoming data. May be null.

sf_data_out

Your function for handling outgoing data. May be null.

sf_connect_in

Your function for handling inbound connections. May be null.

sf_connect_out

Your function for handling outbound connections. May be null.

sf_bind

Your function for handling binds. May be null.

sf_setoption

Your function for handling setsockopt. May be null.

sf_getoption

Your function for handling getsockopt. May be null.

sf_listen

Your function for handling listen. May be null.

sf_ioctl

Your function for handling ioctls. May be null.

sf_len

Length of socket filter extension structure; developers must initialize this to sizeof sflt_filter_ext structure. This field and all fields following it will only be valid if SFLT_EXTENDED flag is set in sf_flags field.

sf_ext_accept

Your function for handling inbound connections at accept time. May be null.

sf_ext_rsvd

Reserved for future use; you must initialize the reserved fields with zeroes.

