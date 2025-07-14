

- GSS
-  gss_krb5_rfc1964_keydata 

Structure

# gss_krb5_rfc1964_keydata

Mac Catalyst 13.0+macOS 10.14+

``` source
struct gss_krb5_rfc1964_keydata
```

## Topics

### Initializers

init()

init(sign_alg: OM_uint32, seal_alg: OM_uint32, ctx_key: gss_krb5_lucid_key_t)

### Instance Properties

var ctx_key: gss_krb5_lucid_key_t

The context key (Kerberos session key or subkey).

var seal_alg: OM_uint32

The seal/encrypt algorithm.

var sign_alg: OM_uint32

The signing algorithm.

## Relationships

### Conforms To

- BitwiseCopyable

## See Also

### Structures

struct gss_krb5_cfx_keydata

struct gss_krb5_lucid_context_v1

struct gss_krb5_lucid_context_version

struct gss_krb5_lucid_key

