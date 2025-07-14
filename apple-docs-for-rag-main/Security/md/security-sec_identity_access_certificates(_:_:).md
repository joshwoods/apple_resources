

- Security
-  sec_identity_access_certificates(\_:\_:) 

Function

# sec_identity_access_certificates(\_:\_:)

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
func sec_identity_access_certificates(
    _ identity: sec_identity_t,
    _ handler: @escaping (sec_certificate_t) -> Void
) -> Bool
```

## Parameters 

`identity`  

A `sec_identity_t` instance.

`handler`  

A block to invoke one or more times with `sec_certificate_t` instances.

## Return Value

Returns true if the peer certificates were accessible, false otherwise.

## Discussion

```
  Access the certificates associated with the `sec_identity_t` instance.
```

