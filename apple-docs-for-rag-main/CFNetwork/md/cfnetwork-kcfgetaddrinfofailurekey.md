

- CFNetwork
-  kCFGetAddrInfoFailureKey 

Global Variable

# kCFGetAddrInfoFailureKey

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+

``` source
let kCFGetAddrInfoFailureKey: CFString
```

## Discussion

If an error of type `kCFHostErrorUnknown` is returned, this key returns the last error code returned by getaddrinfo in response to a DNS lookup. To interpret the results, look up the error code in `/usr/include/netdb.h`.

## See Also

### Constants

let kCFURLErrorFailingURLErrorKey: CFString

The URL that caused the load to fail as a `CFURLRef` object.

let kCFURLErrorFailingURLStringErrorKey: CFString

The URL that caused the load to fail as a `CFStringRef` object.

let kCFSOCKSStatusCodeKey: CFString

let kCFSOCKSVersionKey: CFString

let kCFSOCKSNegotiationMethodKey: CFString

let kCFDNSServiceFailureKey: CFString

let kCFFTPStatusCodeKey: CFString

