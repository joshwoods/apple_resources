

- Foundation
- URLAuthenticationChallenge
-  protectionSpace 

Instance Property

# protectionSpace

The receiver’s protection space.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.2+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
@NSCopying
var protectionSpace: URLProtectionSpace { get }
```

## Mentioned in 

Performing manual server trust authentication

## Discussion

A protection space object provides additional information about the authentication request, such as the host, port, authentication realm, and so on. The protection space also tells you whether the authentication challenge is asking you to provide the user’s credentials or to verify the TLS credentials provided by the server.

