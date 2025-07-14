

- GSS
-  Message Protection 

API Collection

# Message Protection

Provide cryptographic protection to secure message integrity.

## Topics

### Message Wrapping and Verification

Apply a Message Integrity Code (MIC) to a message to guarantee its integrity. Ensure confidentiality using encryption and decryption.

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

func gss_unseal(UnsafeMutablePointer&lt;OM_uint32>, gss_ctx_id_t, gss_buffer_t, gss_buffer_t, UnsafeMutablePointer&lt;Int32>, UnsafeMutablePointer&lt;Int32>) -> OM_uint32

Returns the original version of a secure message by optionally decrypting it and then extracting and verifying the attached MIC.

Deprecated

## See Also

### Messages

Token Management

Establish secure communication with tokens.

Kerberos Implementation

Establish secure connections using the Kerberos implementation of GSS-API.

