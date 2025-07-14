

- Endpoint Security
- es_event_tcc_modify_t
-  init(service:identity:identity_type:update_type:instigator_token:instigator:responsible_token:responsible:right:reason:) 

Initializer

# init(service:identity:identity_type:update_type:instigator_token:instigator:responsible_token:responsible:right:reason:)

Mac CatalystmacOS

``` source
init(
    service: es_string_token_t,
    identity: es_string_token_t,
    identity_type: es_tcc_identity_type_t,
    update_type: es_tcc_event_type_t,
    instigator_token: audit_token_t,
    instigator: UnsafeMutablePointer?,
    responsible_token: UnsafeMutablePointer?,
    responsible: UnsafeMutablePointer?,
    right: es_tcc_authorization_right_t,
    reason: es_tcc_authorization_reason_t
)
```

