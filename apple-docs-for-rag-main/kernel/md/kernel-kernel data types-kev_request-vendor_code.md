

- Kernel
- Kernel Data Types
- kev_request
-  vendor_code 

Instance Property

# vendor_code

All kernel events that don't match this vendor code will be ignored. KEV_ANY_VENDOR can be used to receive kernel events with any vendor code.

macOS 10.9+

``` source
u_int32_t vendor_code;
```

## See Also

### Fields

total_size

Total size of the kernel event message including the header.

kev_class

All kernel events that don't match this class will be ignored. KEV_ANY_CLASS can be used to receive kernel events with any class.

kev_subclass

All kernel events that don't match this subclass will be ignored. KEV_ANY_SUBCLASS can be used to receive kernel events with any subclass.

