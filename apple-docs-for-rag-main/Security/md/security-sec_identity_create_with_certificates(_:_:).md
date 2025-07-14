

- Security
-  sec_identity_create_with_certificates(\_:\_:) 

Function

# sec_identity_create_with_certificates(\_:\_:)

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+macOS 10.14+tvOS 12.0+visionOS 1.0+watchOS 5.0+

``` source
func sec_identity_create_with_certificates(
    _ identity: SecIdentity,
    _ certificates: CFArray
) -> sec_identity_t?
```

## Parameters 

`identity`  

A `SecIdentityRef` instance.

`certificates`  

An array of `SecCertificateRef` instances.

## Return Value

A `sec_identity_t` instance.

## Discussion

```
  Create an ARC-able `sec_identity_t` instance from a `SecIdentityRef` and
  array of SecCertificateRef instances.
```

