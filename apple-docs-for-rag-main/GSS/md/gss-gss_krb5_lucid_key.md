

- GSS
-  gss_krb5_lucid_key 

Structure

# gss_krb5_lucid_key

Mac Catalyst 13.0+macOS 10.14+

``` source
struct gss_krb5_lucid_key
```

## Topics

### Initializers

init()

init(type: OM_uint32, length: OM_uint32, data: UnsafeMutableRawPointer?)

### Instance Properties

var data: UnsafeMutableRawPointer?

The actual key data.

var length: OM_uint32

The length of the key data.

var type: OM_uint32

The key encryption type.

## Relationships

### Conforms To

- BitwiseCopyable

## See Also

### Structures

struct gss_krb5_cfx_keydata

struct gss_krb5_lucid_context_v1

struct gss_krb5_lucid_context_version

struct gss_krb5_rfc1964_keydata

