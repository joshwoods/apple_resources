

- GSS
-  gss_unseal(\_:\_:\_:\_:\_:\_:) Deprecated

Function

# gss_unseal(\_:\_:\_:\_:\_:\_:)

Returns the original version of a secure message by optionally decrypting it and then extracting and verifying the attached MIC.

visionOS 1.0–1.0Deprecated

``` source
func gss_unseal(
    _ minor_status: UnsafeMutablePointer,
    _ context_handle: gss_ctx_id_t,
    _ input_message_buffer: gss_buffer_t,
    _ output_message_buffer: gss_buffer_t,
    _ conf_state: UnsafeMutablePointer,
    _ qop_state: UnsafeMutablePointer
) -> OM_uint32
```

Deprecated

Use gss_unwrap(_:_:_:_:_:_:) instead.

## Parameters 

`minor_status`  

A pointer to the secondary status result that provides additional information in case of failure.

`context_handle`  

The context used to send the message.

`input_message_buffer`  

A buffer containing the protected message from the peer.

`output_message_buffer`  

A buffer the function uses to return the unwrapped message. Release the buffer using a call to gss_release_buffer(_:_:) when you are done with it.

`conf_state`  

A pointer the function uses to indicate what protection had been applied to the message. A value of zero indicates only integrity checking. A non-zero value indicates both integrity checking and confidentiality. Pass `NULL` to ignore this output.

`qop_state`  

A pointer the function uses to return the quality of protection setting. See Quality of Protection Constants in Object Identifiers for valid values. Pass NULL to ignore this output.

## Return Value

A status code set to GSS_S_COMPLETE on success. See Function Status for a complete enumeration of status outputs.

## See Also

### Message Wrapping and Verification

func gss_get_mic(UnsafeMutablePointer&lt;OM_uint32>, gss_ctx_id_t, gss_qop_t, gss_buffer_t, gss_buffer_t) -> OM_uint32

Returns a token that contains the MIC for a message.

func gss_verify_mic(UnsafeMutablePointer&lt;OM_uint32>, gss_ctx_id_t, gss_buffer_t, gss_buffer_t, UnsafeMutablePointer&lt;gss_qop_t>?) -> OM_uint32

Returns an indication of whether the integrity of a message is intact, given its MIC token.

func gss_wrap(UnsafeMutablePointer&lt;OM_uint32>, gss_ctx_id_t, Int32, gss_qop_t, gss_buffer_t, UnsafeMutablePointer&lt;Int32>?, gss_buffer_t) -> OM_uint32

Returns a secure message created by calculating and attaching a MIC to the input message, and then optionally encrypting it.

func gss_unwrap(UnsafeMutablePointer&lt;OM_uint32>, gss_ctx_id_t, gss_buffer_t, gss_buffer_t, UnsafeMutablePointer&lt;Int32>?, UnsafeMutablePointer&lt;gss_qop_t>?) -> OM_uint32

Returns the original version of a secure message by optionally decrypting it and then extracting and verifying the attached MIC.

func gss_sign(UnsafeMutablePointer&lt;OM_uint32>, gss_ctx_id_t, Int32, gss_buffer_t, gss_buffer_t) -> OM_uint32

Returns a digital signature for a message.

Deprecated

func gss_verify(UnsafeMutablePointer&lt;OM_uint32>, gss_ctx_id_t, gss_buffer_t, gss_buffer_t, UnsafeMutablePointer&lt;Int32>) -> OM_uint32

Returns a flag that indicates the integrity of a message’s digital signature.

Deprecated

func gss_seal(UnsafeMutablePointer&lt;OM_uint32>, gss_ctx_id_t, Int32, Int32, gss_buffer_t, UnsafeMutablePointer&lt;Int32>, gss_buffer_t) -> OM_uint32

Returns a secure message created by calculating and attaching a MIC to the input message, and then optionally encrypting it.

Deprecated

