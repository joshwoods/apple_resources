

- Kernel
- Kernel Data Types
-  kev_vendor_code 

# kev_vendor_code

macOS 10.9+

``` source
struct kev_vendor_code {
    ...
};
```

## Discussion

This structure is used with the SIOCGKEVVENDOR ioctl to convert from a string identifying a kext or vendor, in the form of a bundle identifier, to a vendor code.

## Topics

### Fields

vendor_code

After making the SIOCGKEVVENDOR ioctl call, this will be filled in with the vendor code if there is one.

vendor_string

A bundle style identifier.

