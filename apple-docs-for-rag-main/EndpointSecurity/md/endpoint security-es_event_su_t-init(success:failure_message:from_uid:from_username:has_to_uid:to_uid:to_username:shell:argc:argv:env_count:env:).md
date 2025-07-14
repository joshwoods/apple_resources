

- Endpoint Security
- es_event_su_t
-  init(success:failure_message:from_uid:from_username:has_to_uid:to_uid:to_username:shell:argc:argv:env_count:env:) 

Initializer

# init(success:failure_message:from_uid:from_username:has_to_uid:to_uid:to_username:shell:argc:argv:env_count:env:)

Mac CatalystmacOS

``` source
init(
    success: Bool,
    failure_message: es_string_token_t,
    from_uid: uid_t,
    from_username: es_string_token_t,
    has_to_uid: Bool,
    to_uid: es_event_su_t.__Unnamed_union_to_uid,
    to_username: es_string_token_t,
    shell: es_string_token_t,
    argc: Int,
    argv: UnsafeMutablePointer?,
    env_count: Int,
    env: UnsafeMutablePointer?
)
```

