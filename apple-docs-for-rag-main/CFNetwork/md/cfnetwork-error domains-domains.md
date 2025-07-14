

- CFNetwork
-  Error Domains 

API Collection

# Error Domains

High-level error domains.

## Overview

To determine the source of an error, examine the `userInfo` dictionary included in the `CFError` object returned by a function call or call CFErrorGetDomain(_:) and pass in the `CFError` object and the domain whose value you want to read.

## Topics

### Constants

let kCFErrorDomainCFNetwork: CFString

let kCFErrorDomainWinSock: CFString

## See Also

### Errors

enum CFNetworkErrors

This enumeration contains error codes returned under the error domain kCFErrorDomainCFNetwork.

Error Dictionary Keys

Networking-related keys that may be available in a `CFErrorRef` object’s `userInfo` dictionary.

