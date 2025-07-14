

- Kernel
- Kernel Data Types
- kern_event_msg
-  total_size 

Instance Property

# total_size

Total size of the kernel event message including the header.

macOS 10.9+

``` source
u_int32_t total_size;
```

## See Also

### Fields

vendor_code

The vendor code indicates which vendor generated the kernel event. This gives every vendor a unique set of classes and subclasses to use. Use the SIOCGKEVVENDOR ioctl to look up vendor codes for vendors other than Apple. Apple uses KEV_VENDOR_APPLE.

kev_class

The class of the kernel event.

kev_subclass

The subclass of the kernel event.

id

Monotonically increasing value.

event_code

The event code.

event_data

Any additional data about this event. Format will depend on the vendor_code, kev_class, kev_subclass, and event_code. The length of the event_data can be determined using total_size - KEV_MSG_HEADER_SIZE.

