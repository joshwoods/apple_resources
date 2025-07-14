

- Security
- SSLClientCertificateState
-  SSLClientCertificateState.certRejected Deprecated

Case

# SSLClientCertificateState.certRejected

Indicates that the client sent a certificate but the certificate failed validation. This value is seen only on the server side. The server application can inspect the certificate using the function `SSLGetPeerCertificates`.

iOS 2.0–13.0DeprecatediPadOS 2.0–13.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.2–10.15Deprecated

``` source
case certRejected
```

