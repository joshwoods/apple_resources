

- Security
- SecPadding
-  PKCS1SHA224 Deprecated

Type Property

# PKCS1SHA224

Data to be signed is a SHA224 hash.

iOS 2.0–15.0DeprecatediPadOS 2.0–15.0DeprecatedMac Catalyst 13.1–15.0DeprecatedmacOS 10.6–12.0DeprecatedtvOS 4.0–15.0DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 1.0–8.0Deprecated

``` source
static var PKCS1SHA224: SecPadding { get }
```

Deprecated

Replaced with SecKeyAlgorithm

## Discussion

Standard ASN.1 padding will be done, as well as PKCS1 padding of the underlying RSA operation. Used with SecKeyRawSign(_:_:_:_:_:_:) and SecKeyRawVerify(_:_:_:_:_:_:) only.

