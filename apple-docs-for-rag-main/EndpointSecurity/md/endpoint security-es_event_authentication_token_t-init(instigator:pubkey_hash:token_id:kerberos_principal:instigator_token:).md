

- Endpoint Security
- es_event_authentication_token_t
-  init(instigator:pubkey_hash:token_id:kerberos_principal:instigator_token:) 

Initializer

# init(instigator:pubkey_hash:token_id:kerberos_principal:instigator_token:)

Mac CatalystmacOS

``` source
init(
    instigator: UnsafeMutablePointer?,
    pubkey_hash: es_string_token_t,
    token_id: es_string_token_t,
    kerberos_principal: es_string_token_t,
    instigator_token: audit_token_t
)
```

