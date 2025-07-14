

- GSS
-  gss_krb5_copy_ccache(\_:\_:\_:) Deprecated

Function

# gss_krb5_copy_ccache(\_:\_:\_:)

Copies Kerberos 5 credentials into the passed cache.

visionOS 1.0–1.0Deprecated

``` source
func gss_krb5_copy_ccache(
    _ minor_status: UnsafeMutablePointer,
    _ cred: gss_cred_id_t,
    _ out: OpaquePointer
) -> OM_uint32
```

Deprecated

Use gss_export_cred(_:_:_:) instead.

## See Also

### Identity and Settings

func gss_krb5_export_lucid_sec_context(UnsafeMutablePointer&lt;OM_uint32>, UnsafeMutablePointer&lt;gss_ctx_id_t?>, OM_uint32, UnsafeMutablePointer&lt;UnsafeMutableRawPointer>?) -> OM_uint32

Returns a non-opaque version of the internal context information.

func gsskrb5_extract_authz_data_from_sec_context(UnsafeMutablePointer&lt;OM_uint32>, gss_ctx_id_t, Int32, gss_buffer_t) -> OM_uint32

Extracts Kerberos authorization data stored within the context.

func gss_krb5_ccache_name(UnsafeMutablePointer&lt;OM_uint32>, UnsafePointer&lt;CChar>?, UnsafeMutablePointer&lt;UnsafePointer&lt;CChar>?>?) -> OM_uint32

Sets the internal Kerberos 5 credential cache name.

func gss_krb5_free_lucid_sec_context(UnsafeMutablePointer&lt;OM_uint32>, UnsafeMutableRawPointer) -> OM_uint32

Frees allocated storage associated with an exported context.

func gss_krb5_set_allowable_enctypes(UnsafeMutablePointer&lt;OM_uint32>, gss_cred_id_t, OM_uint32, UnsafeMutablePointer&lt;Int32>) -> OM_uint32

Limits the keys that can be exported to the specified types.

func gsskrb5_register_acceptor_identity(UnsafePointer&lt;CChar>) -> OM_uint32

Sets the Kerberos 5 file-based key that the acceptor will use.

func krb5_gss_register_acceptor_identity(UnsafePointer&lt;CChar>) -> OM_uint32

Sets the Kerberos 5 file-based key that the acceptor will use.

