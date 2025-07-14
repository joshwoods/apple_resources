

- Endpoint Security
- es_event_od_group_set_t
-  init(instigator:error_code:group_name:members:node_name:db_path:instigator_token:) 

Initializer

# init(instigator:error_code:group_name:members:node_name:db_path:instigator_token:)

Mac CatalystmacOS

``` source
init(
    instigator: UnsafeMutablePointer?,
    error_code: Int32,
    group_name: es_string_token_t,
    members: UnsafeMutablePointer,
    node_name: es_string_token_t,
    db_path: es_string_token_t,
    instigator_token: audit_token_t
)
```

