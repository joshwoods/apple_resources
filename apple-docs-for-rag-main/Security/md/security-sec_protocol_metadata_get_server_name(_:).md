

- Security
-  sec_protocol_metadata_get_server_name(\_:) 

Function

# sec_protocol_metadata_get_server_name(\_:)

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+macOS 10.14+tvOS 12.0+visionOS 1.0+watchOS 5.0+

``` source
func sec_protocol_metadata_get_server_name(_ metadata: sec_protocol_metadata_t) -> UnsafePointer?
```

## Parameters 

`metadata`  

A `sec_protocol_metadata_t` instance.

## Return Value

Returns A NULL-terminated string carrying the server name, or NULL if none was provided.

## Discussion

```
  Obtain the server name offered by a client or server during
  connection establishmet. This is the value commonly carried
  in the TLS SNI extesion.
```

