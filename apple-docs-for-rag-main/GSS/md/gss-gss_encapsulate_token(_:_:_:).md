

- GSS
-  gss_encapsulate_token(\_:\_:\_:) 

Function

# gss_encapsulate_token(\_:\_:\_:)

Returns a buffer encapsulating the given token.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.7+visionOS 1.0+

``` source
func gss_encapsulate_token(
    _ input_token: gss_const_buffer_t,
    _ oid: gss_const_OID,
    _ output_token: gss_buffer_t
) -> OM_uint32
```

## Parameters 

`input_token`  

A buffer holding the token to be encapsulated.

`oid`  

The token’s object identifier.

`output_token`  

A buffer the function fills with the encapsulated token. Release this buffer’s memory with a call to gss_release_buffer(_:_:) when you are done with it.

## Return Value

A status code set to GSS_S_COMPLETE on success. See Function Status for a complete enumeration of status outputs.

## Discussion

Use this function to encapsulate the initial token of a GSS-API context establishment sequence. It incorporates an identifier of the mechanism type used on that context, and enables unambiguous interpretation of tokens at GSS-API peers.

Use gss_decapsulate_token(_:_:_:) at the peer to reverse the encapsulation.

## See Also

### Encapsulation and Decapsulation

func gss_decapsulate_token(gss_const_buffer_t, gss_const_OID, gss_buffer_t) -> OM_uint32

Returns a token encapsulated in a buffer.

