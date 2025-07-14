

- Kernel
- Kernel Functions
-  kev_vendor_code_find 

Function

# kev_vendor_code_find

macOS 10.9+

``` source
errno_t kev_vendor_code_find(const char *vendor_string, u_int32_t *vendor_code);
```

## Parameters 

`vendor_string`  

A bundle style vendor identifier(i.e. com.apple).

`vendor_code`  

Upon return, a unique vendor code for use when posting kernel events.

## Return Value

May return ENOMEM if memory constraints prevent allocation of a new vendor code.

## Discussion

Lookup a vendor_code given a unique string. If the vendor code has not been used since launch, a unique integer will be assigned for that string. Vendor codes will remain the same until the machine is rebooted.

