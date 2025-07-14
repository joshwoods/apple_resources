

- GSS
-  gss_decapsulate_token(\_:\_:\_:) 

Function

# gss_decapsulate_token(\_:\_:\_:)

Returns a token encapsulated in a buffer.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.7+visionOS 1.0+

``` source
func gss_decapsulate_token(
    _ input_token: gss_const_buffer_t,
    _ oid: gss_const_OID,
    _ output_token: gss_buffer_t
) -> OM_uint32
```

## Parameters 

`input_token`  

A buffer holding the encapsulated token.

`oid`  

The expected object identifier of the token.

`output_token`  

A buffer the function fills with the decapsulated token data. Release this buffer’s memory with a call to gss_release_buffer(_:_:) when you are done with it.

## Return Value

A status code set to GSS_S_COMPLETE on success. See Function Status for a complete enumeration of status outputs.

## Discussion

Use this function to reverse the encapsulation provided by gss_encapsulate_token(_:_:_:).

## See Also

### Encapsulation and Decapsulation

func gss_encapsulate_token(gss_const_buffer_t, gss_const_OID, gss_buffer_t) -> OM_uint32

Returns a buffer encapsulating the given token.

