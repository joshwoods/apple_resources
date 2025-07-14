

- Endpoint Security
- es_event_sudo_t
-  init(success:reject_info:has_from_uid:from_uid:from_username:has_to_uid:to_uid:to_username:command:) 

Initializer

# init(success:reject_info:has_from_uid:from_uid:from_username:has_to_uid:to_uid:to_username:command:)

Mac CatalystmacOS

``` source
init(
    success: Bool,
    reject_info: UnsafeMutablePointer?,
    has_from_uid: Bool,
    from_uid: es_event_sudo_t.__Unnamed_union_from_uid,
    from_username: es_string_token_t,
    has_to_uid: Bool,
    to_uid: es_event_sudo_t.__Unnamed_union_to_uid,
    to_username: es_string_token_t,
    command: es_string_token_t
)
```

