

- GSS
-  gss_krb5_lucid_key_t 

Type Alias

# gss_krb5_lucid_key_t

The structure for a Kerberos encryption key.

Mac Catalyst 13.0+macOS 10.14+

``` source
typealias gss_krb5_lucid_key_t = gss_krb5_lucid_key
```

## Topics

### Key Members

var data: UnsafeMutableRawPointer?

The actual key data.

var length: OM_uint32

The length of the key data.

var type: OM_uint32

The key encryption type.

## See Also

### Contexts and Keys

typealias gss_krb5_cfx_keydata_t

The structure of a Kerberos context and acceptor-asserted key.

typealias gss_krb5_lucid_context_v1_t

The structure of a Kerberos context.

typealias gss_krb5_lucid_context_version_t

The structure for determining the returned Kerberos lucid context structure version.

typealias gss_krb5_rfc1964_keydata_t

The structure for an RFC 1964-compliant Kerberos encryption key.

