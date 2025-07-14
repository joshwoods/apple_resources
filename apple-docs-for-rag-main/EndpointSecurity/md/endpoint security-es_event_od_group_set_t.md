

- Endpoint Security
-  es_event_od_group_set_t 

Structure

# es_event_od_group_set_t

Mac CatalystmacOS

``` source
struct es_event_od_group_set_t
```

## Topics

### Initializers

init(instigator: UnsafeMutablePointer&lt;es_process_t>?, error_code: Int32, group_name: es_string_token_t, members: UnsafeMutablePointer&lt;es_od_member_id_array_t>, node_name: es_string_token_t, db_path: es_string_token_t, instigator_token: audit_token_t)

### Instance Properties

var db_path: es_string_token_t

var error_code: Int32

var group_name: es_string_token_t

var instigator: UnsafeMutablePointer&lt;es_process_t>?

var instigator_token: audit_token_t

var members: UnsafeMutablePointer&lt;es_od_member_id_array_t>

var node_name: es_string_token_t

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

struct es_event_authentication_token_t

struct es_event_authentication_touchid_t

struct es_event_authorization_judgement_t

struct es_event_authorization_petition_t

struct es_event_btm_launch_item_add_t

struct es_event_btm_launch_item_remove_t

struct es_event_gatekeeper_user_override_t

struct es_event_login_login_t

struct es_event_login_logout_t

struct es_event_lw_session_lock_t

