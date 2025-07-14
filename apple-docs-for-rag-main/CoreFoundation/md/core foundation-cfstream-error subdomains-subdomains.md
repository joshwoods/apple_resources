

- Core Foundation
- CFStream
-  Error Subdomains 

# Error Subdomains

Subdomains used to determine how to interpret an error in the `kCFStreamErrorDomainSOCKS` domain.

## Overview

Error codes in the `kCFStreamErrorDomainSOCKS` domain can come from multiple parts of the protocol stack, many of which define their own error values as part of outside specifications such as the HTTP specification.

To avoid confusion from conflicting error numbers, error codes in the `kCFStreamErrorDomainSOCKS` domain contain two parts: a subdomain, which tells which part of the protocol stack generated the error, and the error code itself.

Calling CFSocketStreamSOCKSGetErrorSubdomain(_:) returns an identifier that tells which layer of the protocol stack produced the error. This list of constants contains the possible values that this function will return.

Calling CFSocketStreamSOCKSGetError(_:) returns the actual error code that the subdomain describes.

## Topics

### Constants

var kCFStreamErrorSOCKSSubDomainNone: Int { get }

A general SOCKS error.

var kCFStreamErrorSOCKSSubDomainVersionCode: Int { get }

The version of SOCKS that the server wants to use.

var kCFStreamErrorSOCKS4SubDomainResponse: Int { get }

The SOCKS4 status code returned by the server.

var kCFStreamErrorSOCKS5SubDomainUserPass: Int { get }

The status code that the server returned during authentication.

var kCFStreamErrorSOCKS5SubDomainMethod: Int { get }

The server’s desired negotiation method.

var kCFStreamErrorSOCKS5SubDomainResponse: Int { get }

The response code that the server returned in reply to the connection request.

## See Also

### Constants

enum CFStreamStatus

Constants that describe the status of a stream.

enum CFStreamErrorDomain

Defines constants for values returned in the domain field of the `CFStreamError` structure.

CFStream Error Domain Constants (CFHost)

Defines constants for values returned in the domain field of the `CFStreamError` structure.

Secure Sockets (SOCKS) Errors

Error codes returned by the \`kCFStreamErrorDomainSOCKS\` error domain.

struct CFStreamEventType

Defines constants for stream-related events.

Stream Properties

Stream property names that can be set or copied.

CFStream Property SSL Settings Constants

Constants for use in a `CFDictionary` object that is the value of the `kCFStreamPropertySSLSettings` stream property key.

CFStream Socket Security Level Constants

Constants for setting the security level of a socket stream.

CFStream SOCKS Proxy Key Constants

Constants for SOCKS Proxy `CFDictionary` keys.

Stream Service Types

String constants that specify the service type of a stream.

