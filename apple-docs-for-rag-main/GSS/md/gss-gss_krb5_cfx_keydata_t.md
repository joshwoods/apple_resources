

- GSS
-  gss_krb5_cfx_keydata_t 

Type Alias

# gss_krb5_cfx_keydata_t

The structure of a Kerberos context and acceptor-asserted key.

Mac Catalyst 13.0+macOS 10.14+

``` source
typealias gss_krb5_cfx_keydata_t = gss_krb5_cfx_keydata
```

## Topics

### Key Properties

var acceptor_subkey: gss_krb5_lucid_key_t

The Kerberos session acceptor subkey.

var ctx_key: gss_krb5_lucid_key_t

The Kerberos session context key.

var have_acceptor_subkey: OM_uint32

The flag that indicates if the Kerberos session acceptor subkey is available.

## See Also

### Contexts and Keys

typealias gss_krb5_lucid_context_v1_t

The structure of a Kerberos context.

typealias gss_krb5_lucid_context_version_t

The structure for determining the returned Kerberos lucid context structure version.

typealias gss_krb5_lucid_key_t

The structure for a Kerberos encryption key.

typealias gss_krb5_rfc1964_keydata_t

The structure for an RFC 1964-compliant Kerberos encryption key.

