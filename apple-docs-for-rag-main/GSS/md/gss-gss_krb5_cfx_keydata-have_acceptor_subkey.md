

- GSS
- gss_krb5_cfx_keydata
-  have_acceptor_subkey 

Instance Property

# have_acceptor_subkey

The flag that indicates if the Kerberos session acceptor subkey is available.

Mac Catalyst 13.0+macOS 10.14+

``` source
var have_acceptor_subkey: OM_uint32
```

## Discussion

This flag is set to 1 if the Kerberos session acceptor subkey is available; otherwise, it is set to 0.

## See Also

### Key Properties

var acceptor_subkey: gss_krb5_lucid_key_t

The Kerberos session acceptor subkey.

var ctx_key: gss_krb5_lucid_key_t

The Kerberos session context key.

