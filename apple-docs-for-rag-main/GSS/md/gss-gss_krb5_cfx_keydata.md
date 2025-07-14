

- GSS
-  gss_krb5_cfx_keydata 

Structure

# gss_krb5_cfx_keydata

Mac Catalyst 13.0+macOS 10.14+

``` source
struct gss_krb5_cfx_keydata
```

## Topics

### Initializers

init()

init(have_acceptor_subkey: OM_uint32, ctx_key: gss_krb5_lucid_key_t, acceptor_subkey: gss_krb5_lucid_key_t)

### Instance Properties

var acceptor_subkey: gss_krb5_lucid_key_t

The Kerberos session acceptor subkey.

var ctx_key: gss_krb5_lucid_key_t

The Kerberos session context key.

var have_acceptor_subkey: OM_uint32

The flag that indicates if the Kerberos session acceptor subkey is available.

## Relationships

### Conforms To

- BitwiseCopyable

## See Also

### Structures

struct gss_krb5_lucid_context_v1

struct gss_krb5_lucid_context_version

struct gss_krb5_lucid_key

struct gss_krb5_rfc1964_keydata

