

- GSS
-  gss_krb5_ccache_name(\_:\_:\_:) 

Function

# gss_krb5_ccache_name(\_:\_:\_:)

Sets the internal Kerberos 5 credential cache name.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.7+visionOS 1.0+

``` source
func gss_krb5_ccache_name(
    _ minor_status: UnsafeMutablePointer,
    _ name: UnsafePointer?,
    _ out_name: UnsafeMutablePointer?>?
) -> OM_uint32
```

## See Also

### Identity and Settings

func gss_krb5_export_lucid_sec_context(UnsafeMutablePointer&lt;OM_uint32>, UnsafeMutablePointer&lt;gss_ctx_id_t?>, OM_uint32, UnsafeMutablePointer&lt;UnsafeMutableRawPointer>?) -> OM_uint32

Returns a non-opaque version of the internal context information.

func gsskrb5_extract_authz_data_from_sec_context(UnsafeMutablePointer&lt;OM_uint32>, gss_ctx_id_t, Int32, gss_buffer_t) -> OM_uint32

Extracts Kerberos authorization data stored within the context.

func gss_krb5_free_lucid_sec_context(UnsafeMutablePointer&lt;OM_uint32>, UnsafeMutableRawPointer) -> OM_uint32

Frees allocated storage associated with an exported context.

func gss_krb5_set_allowable_enctypes(UnsafeMutablePointer&lt;OM_uint32>, gss_cred_id_t, OM_uint32, UnsafeMutablePointer&lt;Int32>) -> OM_uint32

Limits the keys that can be exported to the specified types.

func gsskrb5_register_acceptor_identity(UnsafePointer&lt;CChar>) -> OM_uint32

Sets the Kerberos 5 file-based key that the acceptor will use.

func krb5_gss_register_acceptor_identity(UnsafePointer&lt;CChar>) -> OM_uint32

Sets the Kerberos 5 file-based key that the acceptor will use.

func gss_krb5_copy_ccache(UnsafeMutablePointer&lt;OM_uint32>, gss_cred_id_t, OpaquePointer) -> OM_uint32

Copies Kerberos 5 credentials into the passed cache.

Deprecated

