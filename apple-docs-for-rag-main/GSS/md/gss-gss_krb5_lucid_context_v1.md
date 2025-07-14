

- GSS
-  gss_krb5_lucid_context_v1 

Structure

# gss_krb5_lucid_context_v1

Mac Catalyst 13.0+macOS 10.14+

``` source
struct gss_krb5_lucid_context_v1
```

## Topics

### Initializers

init()

init(version: OM_uint32, initiate: OM_uint32, endtime: OM_uint32, send_seq: OM_uint64, recv_seq: OM_uint64, protocol: OM_uint32, rfc1964_kd: gss_krb5_rfc1964_keydata_t, cfx_kd: gss_krb5_cfx_keydata_t)

### Instance Properties

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

## Relationships

### Conforms To

- BitwiseCopyable

## See Also

### Structures

struct gss_krb5_cfx_keydata

struct gss_krb5_lucid_context_version

struct gss_krb5_lucid_key

struct gss_krb5_rfc1964_keydata

