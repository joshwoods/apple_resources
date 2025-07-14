

- Security
-  sec_protocol_metadata_access_pre_shared_keys(\_:\_:) 

Function

# sec_protocol_metadata_access_pre_shared_keys(\_:\_:)

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
func sec_protocol_metadata_access_pre_shared_keys(
    _ metadata: sec_protocol_metadata_t,
    _ handler: @escaping (dispatch_data_t, dispatch_data_t) -> Void
) -> Bool
```

## Parameters 

`metadata`  

A `sec_protocol_metadata_t` instance.

`handler`  

A block to invoke one or more times with tuples of dispatch_data_t objects carrying PSKs and their corresponding identities.

## Return Value

Returns true if the PSKs were accessible, false otherwise.

## Discussion

```
  Get the PSKs supported by the local instance.
```

