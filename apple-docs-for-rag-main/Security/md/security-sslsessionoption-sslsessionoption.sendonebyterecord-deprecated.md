

- Security
- SSLSessionOption
-  SSLSessionOption.sendOneByteRecord Deprecated

Case

# SSLSessionOption.sendOneByteRecord

Enables `1/n-1` record splitting for BEAST attack mitigation.

iOS 2.0–13.0DeprecatediPadOS 2.0–13.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.2–10.15Deprecated

``` source
case sendOneByteRecord
```

## Discussion

When enabled, record splitting is performed only for TLS 1.0 connections based on a block cipher.

