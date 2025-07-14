

- Endpoint Security
- es_process_t
-  init(audit_token:ppid:original_ppid:group_id:session_id:codesigning_flags:is_platform_binary:is_es_client:cdhash:signing_id:team_id:executable:tty:start_time:responsible_audit_token:parent_audit_token:) 

Initializer

# init(audit_token:ppid:original_ppid:group_id:session_id:codesigning_flags:is_platform_binary:is_es_client:cdhash:signing_id:team_id:executable:tty:start_time:responsible_audit_token:parent_audit_token:)

Mac CatalystmacOS

``` source
init(
    audit_token: audit_token_t,
    ppid: pid_t,
    original_ppid: pid_t,
    group_id: pid_t,
    session_id: pid_t,
    codesigning_flags: UInt32,
    is_platform_binary: Bool,
    is_es_client: Bool,
    cdhash: es_cdhash_t,
    signing_id: es_string_token_t,
    team_id: es_string_token_t,
    executable: UnsafeMutablePointer,
    tty: UnsafeMutablePointer?,
    start_time: timeval,
    responsible_audit_token: audit_token_t,
    parent_audit_token: audit_token_t
)
```

