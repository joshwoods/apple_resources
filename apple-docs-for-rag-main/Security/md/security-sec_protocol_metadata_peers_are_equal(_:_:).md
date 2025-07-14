

- Security
-  sec_protocol_metadata_peers_are_equal(\_:\_:) 

Function

# sec_protocol_metadata_peers_are_equal(\_:\_:)

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+macOS 10.14+tvOS 12.0+visionOS 1.0+watchOS 5.0+

``` source
func sec_protocol_metadata_peers_are_equal(
    _ metadataA: sec_protocol_metadata_t,
    _ metadataB: sec_protocol_metadata_t
) -> Bool
```

## Parameters 

`metadataA`  

A `sec_protocol_metadata_t` instance.

`metadataB`  

A `sec_protocol_metadata_t` instance.

## Return Value

Returns true if both metadata values refer to the same peer, and false otherwise.

## Discussion

```
  Compare peer information for two `sec_protocol_metadata` instances.
  This comparison does not include protocol configuration options, e.g., ciphersuites.
```

