

- Security
-  sec_certificate_copy_ref(\_:) 

Function

# sec_certificate_copy_ref(\_:)

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+macOS 10.14+tvOS 12.0+visionOS 1.0+watchOS 5.0+

``` source
func sec_certificate_copy_ref(_ certificate: sec_certificate_t) -> Unmanaged
```

## Parameters 

`certificate`  

A `sec_certificate_t` instance.

## Return Value

The underlying `SecCertificateRef` instance.

## Discussion

```
  Copy a retained reference to the underlying `SecCertificateRef` instance.
```

