

- GSS
-  gss_sign(\_:\_:\_:\_:\_:) Deprecated

Function

# gss_sign(\_:\_:\_:\_:\_:)

Returns a digital signature for a message.

visionOS 1.0–1.0Deprecated

``` source
func gss_sign(
    _ minor_status: UnsafeMutablePointer,
    _ context_handle: gss_ctx_id_t,
    _ qop_req: Int32,
    _ message_buffer: gss_buffer_t,
    _ message_token: gss_buffer_t
) -> OM_uint32
```

Deprecated

Use gss_get_mic(_:_:_:_:_:) instead.

## Parameters 

`minor_status`  

A pointer to the secondary status result that provides additional information in case of failure.

`context_handle`  

The context used to send the message.

`qop_req`  

The quality of protection requested for the message. See Quality of Protection Constants for valid values.

`message_buffer`  

A buffer holding the message to be protected.

`message_token`  

A buffer the function fills with the protection token. Release this buffer with a call to gss_release_buffer(_:_:) when you are done with it.

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

func gss_verify(UnsafeMutablePointer&lt;OM_uint32>, gss_ctx_id_t, gss_buffer_t, gss_buffer_t, UnsafeMutablePointer&lt;Int32>) -> OM_uint32

Returns a flag that indicates the integrity of a message’s digital signature.

Deprecated

func gss_seal(UnsafeMutablePointer&lt;OM_uint32>, gss_ctx_id_t, Int32, Int32, gss_buffer_t, UnsafeMutablePointer&lt;Int32>, gss_buffer_t) -> OM_uint32

Returns a secure message created by calculating and attaching a MIC to the input message, and then optionally encrypting it.

Deprecated

func gss_unseal(UnsafeMutablePointer&lt;OM_uint32>, gss_ctx_id_t, gss_buffer_t, gss_buffer_t, UnsafeMutablePointer&lt;Int32>, UnsafeMutablePointer&lt;Int32>) -> OM_uint32

Returns the original version of a secure message by optionally decrypting it and then extracting and verifying the attached MIC.

Deprecated

