

- CFNetwork
-  kCFSOCKSVersionKey 

Global Variable

# kCFSOCKSVersionKey

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+

``` source
let kCFSOCKSVersionKey: CFString
```

## Discussion

If an error of type `kCFSOCKSErrorUnsupportedServerVersion` is returned, querying this key returns the SOCKS version in use by the current connection.

## See Also

### Constants

let kCFURLErrorFailingURLErrorKey: CFString

The URL that caused the load to fail as a `CFURLRef` object.

let kCFURLErrorFailingURLStringErrorKey: CFString

The URL that caused the load to fail as a `CFStringRef` object.

let kCFGetAddrInfoFailureKey: CFString

let kCFSOCKSStatusCodeKey: CFString

let kCFSOCKSNegotiationMethodKey: CFString

let kCFDNSServiceFailureKey: CFString

let kCFFTPStatusCodeKey: CFString

