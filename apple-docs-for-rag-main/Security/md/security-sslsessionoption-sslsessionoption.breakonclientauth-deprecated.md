

- Security
- SSLSessionOption
-  SSLSessionOption.breakOnClientAuth Deprecated

Case

# SSLSessionOption.breakOnClientAuth

Enables returning from SSLHandshake(_:) (with a result of `errSSLClientAuthCompleted`) when the client authentication portion of the handshake is complete to allow your application to perform its own certificate verification.

iOS 2.0–13.0DeprecatediPadOS 2.0–13.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.2–10.15Deprecated

``` source
case breakOnClientAuth
```

## Discussion

Note that in iOS (all versions) and macOS 10.8 and later, setting this option disables Secure Transport’s automatic verification of client certificates.

If you set this option, your application should perform its own certificate verification when `errSSLClientAuthCompleted` is returned before continuing with the handshake.

