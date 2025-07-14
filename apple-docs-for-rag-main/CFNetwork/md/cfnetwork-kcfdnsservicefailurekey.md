

- CFNetwork
-  kCFDNSServiceFailureKey 

Global Variable

# kCFDNSServiceFailureKey

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+

``` source
let kCFDNSServiceFailureKey: CFString
```

## Discussion

If an error of type `kCFNetServicesErrorDNSServiceFailure` is returned, querying this key returns the last error returned by the DNS resolver libraries in response to the previous operation. To interpret the results, look up the error codes in `/usr/include/dns_sd.h` or DNS Service Discovery C.

## See Also

### Constants

let kCFURLErrorFailingURLErrorKey: CFString

The URL that caused the load to fail as a `CFURLRef` object.

let kCFURLErrorFailingURLStringErrorKey: CFString

The URL that caused the load to fail as a `CFStringRef` object.

let kCFGetAddrInfoFailureKey: CFString

let kCFSOCKSStatusCodeKey: CFString

let kCFSOCKSVersionKey: CFString

let kCFSOCKSNegotiationMethodKey: CFString

let kCFFTPStatusCodeKey: CFString

