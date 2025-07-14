

- Security
-  sec_certificate_create(\_:) 

Function

# sec_certificate_create(\_:)

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+macOS 10.14+tvOS 12.0+visionOS 1.0+watchOS 5.0+

``` source
func sec_certificate_create(_ certificate: SecCertificate) -> sec_certificate_t?
```

## Parameters 

`certificate`  

A `SecCertificateRef` instance.

## Return Value

A `sec_certificate_t` instance.

## Discussion

```
  Create an ARC-able `sec_certificate_t` instance from a `SecCertificateRef`.
```

