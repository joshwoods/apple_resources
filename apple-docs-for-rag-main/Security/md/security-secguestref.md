

- Security
-  SecGuestRef 

Type Alias

# SecGuestRef

A reference to a guest object, which identifies a particular block of guest code in the context of its code signing host.

Mac Catalyst 13.0+macOS 10.0+

``` source
typealias SecGuestRef = UInt32
```

## Discussion

Guest handles are assigned by the host at will, with kSecNoGuest being reserved as the `NULL` value. They can be reused for new children if desired.

