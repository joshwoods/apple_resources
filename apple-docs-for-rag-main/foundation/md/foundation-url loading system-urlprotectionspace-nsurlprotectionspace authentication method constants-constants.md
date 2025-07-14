

- Foundation
- URL Loading System
- URLProtectionSpace
-  NSURLProtectionSpace authentication method constants 

API Collection

# NSURLProtectionSpace authentication method constants

Constants describing known values of the authenticationMethod property of a URLProtectionSpace.

## Overview

These constants are also used with the URLProtectionSpace initializers init(host:port:protocol:realm:authenticationMethod:) and init(proxyHost:port:type:realm:authenticationMethod:).

## Topics

### Session-wide authentication challenges

These constants indicate session-wide challenges. Delegates handle these challenges in the URLSessionDelegate method urlSession(_:didReceive:completionHandler:).

let NSURLAuthenticationMethodClientCertificate: String

Use client certificate authentication for this protection space.

let NSURLAuthenticationMethodNegotiate: String

Negotiate whether to use Kerberos or NTLM authentication for this protection space.

let NSURLAuthenticationMethodNTLM: String

Use NTLM authentication for this protection space.

let NSURLAuthenticationMethodServerTrust: String

Perform server trust authentication (certificate validation) for this protection space.

### Task-specific authentication challenges

These constants indicate task-specific challenges. Delegates handle these challenges in the URLSessionTaskDelegate method urlSession(_:task:didReceive:completionHandler:).

let NSURLAuthenticationMethodDefault: String

Use the default authentication method for a protocol.

let NSURLAuthenticationMethodHTMLForm: String

Use HTML form authentication for this protection space.

let NSURLAuthenticationMethodHTTPBasic: String

Use HTTP basic authentication for this protection space.

let NSURLAuthenticationMethodHTTPDigest: String

Use HTTP digest authentication for this protection space.

## See Also

### Related Documentation

Handling an authentication challenge

Respond appropriately when a server demands authentication for a URL request.

Performing manual server trust authentication

Evaluate the server’s security credentials in your app.

### Identifying protection space properties

NSURLProtectionSpace protocol types

These constants describe the supported protocols for a protection space, as returned by protocol.

NSURLProtectionSpace proxy types

These constants describe the supported proxy types used in init(proxyHost:port:type:realm:authenticationMethod:) and returned by proxyType.

