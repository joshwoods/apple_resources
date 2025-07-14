

- Security
-  sec_protocol_metadata_create_secret(\_:\_:\_:\_:) 

Function

# sec_protocol_metadata_create_secret(\_:\_:\_:\_:)

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+macOS 10.14+tvOS 12.0+visionOS 1.0+watchOS 5.0+

``` source
func sec_protocol_metadata_create_secret(
    _ metadata: sec_protocol_metadata_t,
    _ label_len: Int,
    _ label: UnsafePointer,
    _ exporter_length: Int
) -> dispatch_data_t?
```

## Parameters 

`metadata`  

A `sec_protocol_metadata_t` instance.

`label_len`  

Length of the KDF label string.

`label`  

KDF label string.

`exporter_length`  

Length of the secret to be exported.

## Return Value

Returns a dispatch_data_t object carrying the exported secret.

## Discussion

```
  Export a secret, e.g., a cryptographic key, derived from the protocol metadata using a label string.
```

