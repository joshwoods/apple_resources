

- Security
-  sec_protocol_metadata_access_ocsp_response(\_:\_:) 

Function

# sec_protocol_metadata_access_ocsp_response(\_:\_:)

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+macOS 10.14+tvOS 12.0+visionOS 1.0+watchOS 5.0+

``` source
func sec_protocol_metadata_access_ocsp_response(
    _ metadata: sec_protocol_metadata_t,
    _ handler: @escaping (dispatch_data_t) -> Void
) -> Bool
```

## Parameters 

`metadata`  

A `sec_protocol_metadata_t` instance.

`handler`  

A block to invoke one or more times with OCSP data

## Return Value

Returns true if the OSCP response was accessible, false otherwise.

## Discussion

```
  Get the OCSP response from the protocol instance peer.
```

