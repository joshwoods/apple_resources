

- Endpoint Security
-  es_event_authentication_token_t 

Structure

# es_event_authentication_token_t

Mac CatalystmacOS

``` source
struct es_event_authentication_token_t
```

## Topics

### Initializers

init()

init(instigator: UnsafeMutablePointer&lt;es_process_t>?, pubkey_hash: es_string_token_t, token_id: es_string_token_t, kerberos_principal: es_string_token_t, instigator_token: audit_token_t)

### Instance Properties

var instigator: UnsafeMutablePointer&lt;es_process_t>?

var instigator_token: audit_token_t

var kerberos_principal: es_string_token_t

var pubkey_hash: es_string_token_t

var token_id: es_string_token_t

## Relationships

### Conforms To

- BitwiseCopyable

## See Also

### Structures

struct es_authorization_result_t

struct es_btm_launch_item_t

struct es_event_authentication_auto_unlock_t

struct es_event_authentication_od_t

struct es_event_authentication_t

struct es_event_authentication_touchid_t

struct es_event_authorization_judgement_t

struct es_event_authorization_petition_t

struct es_event_btm_launch_item_add_t

struct es_event_btm_launch_item_remove_t

struct es_event_gatekeeper_user_override_t

struct es_event_login_login_t

struct es_event_login_logout_t

struct es_event_lw_session_lock_t

struct es_event_lw_session_login_t

