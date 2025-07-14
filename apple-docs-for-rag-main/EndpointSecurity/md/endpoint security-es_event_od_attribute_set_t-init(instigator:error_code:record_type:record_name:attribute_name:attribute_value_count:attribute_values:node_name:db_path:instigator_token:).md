

- Endpoint Security
- es_event_od_attribute_set_t
-  init(instigator:error_code:record_type:record_name:attribute_name:attribute_value_count:attribute_values:node_name:db_path:instigator_token:) 

Initializer

# init(instigator:error_code:record_type:record_name:attribute_name:attribute_value_count:attribute_values:node_name:db_path:instigator_token:)

Mac CatalystmacOS

``` source
init(
    instigator: UnsafeMutablePointer?,
    error_code: Int32,
    record_type: es_od_record_type_t,
    record_name: es_string_token_t,
    attribute_name: es_string_token_t,
    attribute_value_count: Int,
    attribute_values: UnsafeMutablePointer?,
    node_name: es_string_token_t,
    db_path: es_string_token_t,
    instigator_token: audit_token_t
)
```

