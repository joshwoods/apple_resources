

- Foundation
-  NSURLAuthenticationMethodServerTrust 

Global Variable

# NSURLAuthenticationMethodServerTrust

Perform server trust authentication (certificate validation) for this protection space.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.6+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
let NSURLAuthenticationMethodServerTrust: String
```

## Mentioned in 

Performing manual server trust authentication

## Discussion

This authentication method can apply to any protocol, and is most commonly used for overriding SSL and TLS chain validation.

To learn more, read Overriding TLS Chain Validation Correctly.

## See Also

### Session-wide authentication challenges

let NSURLAuthenticationMethodClientCertificate: String

Use client certificate authentication for this protection space.

let NSURLAuthenticationMethodNegotiate: String

Negotiate whether to use Kerberos or NTLM authentication for this protection space.

let NSURLAuthenticationMethodNTLM: String

Use NTLM authentication for this protection space.

