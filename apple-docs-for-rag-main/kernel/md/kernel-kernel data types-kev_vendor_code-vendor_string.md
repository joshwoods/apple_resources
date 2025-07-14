

- Kernel
- Kernel Data Types
- kev_vendor_code
-  vendor_string 

Instance Property

# vendor_string

A bundle style identifier.

macOS 10.9+

``` source
char vendor_string[200];
```

## See Also

### Fields

vendor_code

After making the SIOCGKEVVENDOR ioctl call, this will be filled in with the vendor code if there is one.

