

- Security
-  kSecGuestAttributeCanonical 

Global Variable

# kSecGuestAttributeCanonical

A key whose value is the guest code object for that guest.

Mac Catalyst 13.0+macOS 10.0+

``` source
let kSecGuestAttributeCanonical: CFString
```

## Discussion

This object plus the process ID (kSecGuestAttributePid) uniquely identify the guest.

