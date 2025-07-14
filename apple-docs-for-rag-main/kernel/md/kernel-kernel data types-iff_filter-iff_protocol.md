

- Kernel
- Kernel Data Types
- iff_filter
-  iff_protocol 

Instance Property

# iff_protocol

The protocol of the packets this filter is interested in. If you specify zero, packets from all protocols will be passed to the filter.

macOS 10.6+

``` source
protocol_family_t iff_protocol;
```

## See Also

### Fields

iff_cookie

A kext defined cookie that will be passed to all filter functions.

iff_name

A filter name used for debugging purposes.

iff_input

The filter function to handle inbound packets, may be NULL.

iff_output

The filter function to handle outbound packets, may be NULL.

iff_event

The filter function to handle interface events, may be null.

iff_ioctl

The filter function to handle interface ioctls, may be null.

iff_detached

The filter function used to notify the filter that it has been detached.

