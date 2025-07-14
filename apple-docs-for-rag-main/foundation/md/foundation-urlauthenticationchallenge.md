

- Foundation
-  URLAuthenticationChallenge 

Class

# URLAuthenticationChallenge

A challenge from a server requiring authentication from the client.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.2+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
class URLAuthenticationChallenge
```

## Overview

Your app receives authentication challenges in various URLSession, NSURLConnection, and NSURLDownload delegate methods, such as urlSession(_:task:didReceive:completionHandler:). These objects provide the information you’ll need when deciding how to handle a server’s request for authentication.

At the core of that authentication challenge is a *protection space* that defines the type of authentication being requested, the host and port number, the networking protocol, and (where applicable) the authentication realm (a group of related URLs on the same server that share a single set of credentials).

## Topics

### Creating an authentication challenge instance

init(authenticationChallenge: URLAuthenticationChallenge, sender: any URLAuthenticationChallengeSender)

Creates an authentication challenge from an existing challenge instance.

init(protectionSpace: URLProtectionSpace, proposedCredential: URLCredential?, previousFailureCount: Int, failureResponse: URLResponse?, error: (any Error)?, sender: any URLAuthenticationChallengeSender)

Initializes an authentication challenge from parameters you provide.

### Inspecting the authentication challenge

var protectionSpace: URLProtectionSpace

The receiver’s protection space.

### Getting properties of previous authentication attempts

var failureResponse: URLResponse?

The URL response object representing the last authentication failure.

var previousFailureCount: Int

The receiver’s count of failed authentication attempts.

var proposedCredential: URLCredential?

The proposed credential for this challenge.

### Getting authentication errors

var error: (any Error)?

The error object representing the last authentication failure.

### Legacy

var sender: (any URLAuthenticationChallengeSender)?

The sender of the challenge.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSObjectProtocol
- NSSecureCoding
- Sendable

## See Also

### Authentication and credentials

Handling an authentication challenge

Respond appropriately when a server demands authentication for a URL request.

class URLCredential

`A`n authentication credential consisting of information specific to the type of credential and the type of persistent storage to use, if any.

class URLCredentialStorage

The manager of a shared credentials cache.

class URLProtectionSpace

A server or an area on a server, commonly referred to as a realm, that requires authentication.

