

- GSS
-  gss_krb5_lucid_context_v1_t 

Type Alias

# gss_krb5_lucid_context_v1_t

The structure of a Kerberos context.

Mac Catalyst 13.0+macOS 10.14+

``` source
typealias gss_krb5_lucid_context_v1_t = gss_krb5_lucid_context_v1
```

## Topics

### Context Members

var cfx_kd: gss_krb5_cfx_keydata_t

The key data structure for Kerberos 5.

var endtime: OM_uint32

The expiration time of the context.

var initiate: OM_uint32

The flag indicating if the role is initiator.

var `protocol`: OM_uint32

The protocol to use.

var recv_seq: OM_uint64

The receive sequence number.

var rfc1964_kd: gss_krb5_rfc1964_keydata_t

The RFC-1964 key data.

var send_seq: OM_uint64

The send sequence number.

var version: OM_uint32

The structure version number.

## See Also

### Contexts and Keys

typealias gss_krb5_cfx_keydata_t

The structure of a Kerberos context and acceptor-asserted key.

typealias gss_krb5_lucid_context_version_t

The structure for determining the returned Kerberos lucid context structure version.

typealias gss_krb5_lucid_key_t

The structure for a Kerberos encryption key.

typealias gss_krb5_rfc1964_keydata_t

The structure for an RFC 1964-compliant Kerberos encryption key.

