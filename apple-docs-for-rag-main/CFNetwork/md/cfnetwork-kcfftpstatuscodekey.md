

- CFNetwork
-  kCFFTPStatusCodeKey 

Global Variable

# kCFFTPStatusCodeKey

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+

``` source
let kCFFTPStatusCodeKey: CFString
```

## Discussion

If an error of type `kCFFTPErrorUnexpectedStatusCode` is returned, querying this key returns the last status code sent by the FTP server in response to the previous operation.

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

let kCFDNSServiceFailureKey: CFString

