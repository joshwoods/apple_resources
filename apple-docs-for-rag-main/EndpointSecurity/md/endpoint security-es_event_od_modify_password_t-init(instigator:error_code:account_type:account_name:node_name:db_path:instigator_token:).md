

- Endpoint Security
- es_event_od_modify_password_t
-  init(instigator:error_code:account_type:account_name:node_name:db_path:instigator_token:) 

Initializer

# init(instigator:error_code:account_type:account_name:node_name:db_path:instigator_token:)

Mac CatalystmacOS

``` source
init(
    instigator: UnsafeMutablePointer?,
    error_code: Int32,
    account_type: es_od_account_type_t,
    account_name: es_string_token_t,
    node_name: es_string_token_t,
    db_path: es_string_token_t,
    instigator_token: audit_token_t
)
```

