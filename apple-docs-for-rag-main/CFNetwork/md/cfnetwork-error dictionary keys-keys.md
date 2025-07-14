

- CFNetwork
-  Error Dictionary Keys 

API Collection

# Error Dictionary Keys

Networking-related keys that may be available in a `CFErrorRef` object’s `userInfo` dictionary.

## Overview

Many network functions return `CFErrorRef` objects. When the error object’s domain is `kCFErrorDomainCFNetwork`, you can query the object for additional information.

For example:

```
```

## Topics

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

let kCFFTPStatusCodeKey: CFString

## See Also

### Errors

enum CFNetworkErrors

This enumeration contains error codes returned under the error domain kCFErrorDomainCFNetwork.

Error Domains

High-level error domains.

