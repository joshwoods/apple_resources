

- Endpoint Security
-  es_event_sudo_t 

Structure

# es_event_sudo_t

Mac CatalystmacOS

``` source
struct es_event_sudo_t
```

## Topics

### Initializers

init()

init(success: Bool, reject_info: UnsafeMutablePointer&lt;es_sudo_reject_info_t>?, has_from_uid: Bool, from_uid: es_event_sudo_t.__Unnamed_union_from_uid, from_username: es_string_token_t, has_to_uid: Bool, to_uid: es_event_sudo_t.__Unnamed_union_to_uid, to_username: es_string_token_t, command: es_string_token_t)

### Instance Properties

var command: es_string_token_t

var from_uid: es_event_sudo_t.__Unnamed_union_from_uid

var from_username: es_string_token_t

var has_from_uid: Bool

var has_to_uid: Bool

var reject_info: UnsafeMutablePointer&lt;es_sudo_reject_info_t>?

var success: Bool

var to_uid: es_event_sudo_t.__Unnamed_union_to_uid

var to_username: es_string_token_t

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

