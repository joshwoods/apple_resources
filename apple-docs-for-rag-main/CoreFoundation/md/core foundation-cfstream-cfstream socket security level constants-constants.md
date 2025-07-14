

- Core Foundation
- CFStream
-  CFStream Socket Security Level Constants 

API Collection

# CFStream Socket Security Level Constants

Constants for setting the security level of a socket stream.

## Overview

This enumeration defines the preferred constants for setting the security protocol for a socket stream pair when calling CFReadStreamSetProperty(_:_:_:) or CFWriteStreamSetProperty(_:_:_:).

## Topics

### Constants

let kCFStreamSocketSecurityLevelNone: CFString

Specifies that no security level be set.

let kCFStreamSocketSecurityLevelSSLv2: CFString

Specifies that SSL version 2 be set as the security protocol for a socket stream.

Deprecated

let kCFStreamSocketSecurityLevelSSLv3: CFString

Specifies that SSL version 3 be set as the security protocol for a socket stream pair.

Deprecated

let kCFStreamSocketSecurityLevelTLSv1: CFString

Specifies that TLS version 1 be set as the security protocol for a socket stream.

let kCFStreamSocketSecurityLevelNegotiatedSSL: CFString

Specifies that the highest level security protocol that can be negotiated be set as the security protocol for a socket stream.

## See Also

### Setting the Security Protocol

func CFReadStreamSetProperty(CFReadStream!, CFStreamPropertyKey!, CFTypeRef!) -> Bool

Sets the value of a property for a stream.

func CFWriteStreamSetProperty(CFWriteStream!, CFStreamPropertyKey!, CFTypeRef!) -> Bool

Sets the value of a property for a stream.

